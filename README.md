# talleraws
# Ingresar a la consola de AWS 
https://console.aws.amazon.com/

## 1.- Crear lambda function
Function name: Demo<br>
Runtime: python 3.7<br> 
Create function<br>
## 2.- Abrir lambda Demo
Function code agregar:<br>
<pre>
        'body': json.dumps('Hello from Lambda!',
        'headers': {
            'Content-type': 'application/json',
        },
</pre>
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
        API endpoint: https://xxxxxxxx.execute-api.us-east-1.amazonaws.com/default/Demo   <-- (Click)
</pre>


