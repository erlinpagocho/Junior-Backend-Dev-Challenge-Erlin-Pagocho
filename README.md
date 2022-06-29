# Junior-Backend-Dev-Challenge-Erlin-Pagocho

API  DE GESTÃO DE DADOS DE UM FUNCIONÁRIO

Para poder testar os serviços é necessário instalar as ferramentas:
- Eclipse
- Postman

Passo:
 1. Importar o projecto no eclipse


* Para Criar um funcionário com todos os atributos necessários.
NOTA: O Nuit é único para cada funcionario

Passos:
  1. Subir a api no eclipse
  2. No Postman e incluir os dados abaixos mencionados
 
	URL:
	 (POST):localhost:8080/funcionario/createFuncionario?

	HEADERS:
	 Key: Content-Type
	 Value: application/json
	
	BODY:
	{   
    	"name": "Erlin",
    	"surname": "Pagocho",
    	"birthDate":"12/05/1997",
    	"civil_status":"solteiro",
    	"identificationDocument":"BI", 
    	"nuit":"110857578",
    	"email": "ecpp24@gmail.com" ,
    	"contact" : "845505331"
	}
  3. Clicar Send



* Com a Url abaixo é possivel Listar todos funcionários existentes.

Passos:
  1. Subir a api no eclipse
  2. Abrir o Postman e Incluir a Url e clicar Send 
     Url(GET): localhost:8080/funcionario/findAll

* Pegar dados de um determinado funcionário.
Passos:
  1. Subir a api no eclipse
  2. Abrir o Postman e Incluir a Url abaixo, 
     no qual tem 2 possibilidades, pegar pelo ID ou pegar pelo Nuit.

   Url(GET): localhost:8080/funcionario/findByNuit/110857578

   ou

   Url(GET): localhost:8080/funcionario/findById/1

* Atualizar dados de um determinado funcionário, a actualização de dados pode ser feita 
 de 2 maneiras, pelo ID ou pelo Nuit, no qual se incluir o ID ou pelo Nuit.

Passos:
  1. Subir a api no eclipse
  2. No Postman e incluir os dados abaixos mencionados
 
	URL:
	 (POST):localhost:8080/funcionario/updateFuncionario?

	HEADERS:
	 Key: Content-Type
	 Value: application/json
	
	BODY:
	{  
    	"id": "1"
   	"name": "Erlin",
    	"surname": "Pagocho",
    	"birthDate":"12/05/1997",
    	"civil_status":"solteiro",
    	"identificationDocument":"BI", 
    	"nuit":"110857578",
    	"email": "ecpp24@gmail.com" ,
    	"contact" : "845505331"
	}

	ou

	{  
    	"name": "Erlin",
    	"surname": "Pagocho",
    	"birthDate":"12/05/1997",
    	"civil_status":"solteiro",
    	"identificationDocument":"BI", 
    	"nuit":"110857578",
    	"email": "ecpp24@gmail.com" ,
    	"contact" : "845505331"
	}

* Para Eliminar um determinado funcionário é possivel o fazer de 2 maneiras,
  pelo ID ou pelo Nuit.

Passos:
  1. Subir a api no eclipse
  2. No Postman e incluir os dados abaixos mencionados
 
 Url(DELETE): localhost:8080/funcionario/deleteByNuit/110857578

ou

 Url(DELETE): localhost:8080/funcionario/deleteById/1


* Inactivar um determinado funcionário, caso se deseje inactivar e não apagar um funcionario,
 no qual também é possivel o fazer informando o ID ou o Nuit.

Passos:
  1. Subir a api no eclipse
  2. No Postman e incluir os dados abaixos mencionados
 
Url(POST): localhost:8080/funcionario/inactivateByNuit/110857578

ou

Url(POST): localhost:8080/funcionario/inactivateById/1
