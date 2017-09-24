# FCM_InterfaceWEB_1




Referencia : https://github.com/firebase/quickstart-js/tree/master/messaging 


Diretorio : C:\Users\lprates\Desktop\fcm\quickstart-js-master\messaging


Para Rodar Por meio de javascript 


1 - Instalar CLI : 

	npm install -g firebase-tools
 

2 - Autenticar 
 
	firebase login --interactive

3 - Listar Projetos 

	firebase list
	
4 - Usar projeto 

	firebase use projetofcm-ae622	
	
5 - Executar projeto 

firebase serve -p 8081	
	
6 - Acessar e dar permissao 

http://localhost:8081 	

7- Pegar Token e enviar Mensagem 

Token 

cYJmyAugQbE:APA91bH_SfAJ-hJXrxsByOsf0A46hDlkMpXWgfTUI9cmKcPn4nu-ysjQ5DZsyxtxDvRgYq3YiamWYAKgiIS0ETjhNJoXEPtJYGMatPDOPxP8s27kfEIFKsZ8BDwmMAOw7Uir8sLKxcmK


8 - Enviar POST 


POST /fcm/send HTTP/1.1
Host: fcm.googleapis.com
Authorization: key=AAAAGYw4hd8:APA91bG_vtOqwjhgXCbtwLltqUJuWSIF_H4ScHybfNhWoJ5JNxEnLKogPwyzfpHZidfn4H95jO88ViSaI7mgJLnm7K9fqrch8Ma-R-pbRaS1slspAum7UmBsa5ljbxJc1EUtDNWRt0CN
Content-Type: application/json

```json 

{
  "notification": {
    "title": "Portugal vs. Denmark",
    "body": "5 to 1",
    "icon": "firebase-logo.png",
    "click_action": "http://localhost:8081"
  },
  "to": "cYJmyAugQbE:APA91bH_SfAJ-hJXrxsByOsf0A46hDlkMpXWgfTUI9cmKcPn4nu-ysjQ5DZsyxtxDvRgYq3YiamWYAKgiIS0ETjhNJoXEPtJYGMatPDOPxP8s27kfEIFKsZ8BDwmMAOw7Uir8sLKxcmK"
}

```



