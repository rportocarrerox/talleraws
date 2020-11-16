# talleraws
# Ingresar a la consola de AWS 
https://console.aws.amazon.com/

## 1.- Crear lambda function
Function name: Demo<br>
Runtime: python 3.7<br> 
Create function<br>
## 2.- Abrir lambda Demo
## 3.- Add Trigger
<pre>
        Trigger configuration: API Gateway
        API: Create API
        API Type: Rest API
        Security: Open
        Add
        
</pre>

## 4.- API Gateway
<pre>
Details:
        API endpoint: https://xxxxxxxx.execute-api.us-east-1.amazonaws.com/default/Demo   <-- (Right click new tab)
        curl https://xxxxxxxx.execute-api.us-east-1.amazonaws.com/default/Demo
</pre>

## 5.- Function code
<pre>
### Cambiar Hello Word! por Taller Ninja
lambda_function:
        'body': json.dumps('Taller ninja!')
        Deploy
        curl https://xxxxxxxx.execute-api.us-east-1.amazonaws.com/default/Demo
</pre>
