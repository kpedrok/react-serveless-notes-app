# serverless_stack

App client id
30cvhbm2p8mvmmogpl2a9lkiir

aws cognito-idp sign-up --region us-east-1 --client-id 30cvhbm2p8mvmmogpl2a9lkiir --username pedro@taglivros.com.br --password Passw0rd!

{
"UserConfirmed": false,
"CodeDeliveryDetails": {
"Destination": "p**_@t_**.br",
"DeliveryMedium": "EMAIL",
"AttributeName": "email"
},
"UserSub": "7592da8b-957f-4ad4-be8c-6226b5cf658d"
}

aws cognito-idp admin-confirm-sign-up --region us-east-1 --user-pool-id us-east-1_u0WhuIEDY --username pedro@taglivros.com.br

{
"statusCode": 200,
"headers": {
"Access-Control-Allow-Origin": "\*",
"Access-Control-Allow-Credentials": true
},
"body": "{\"userId\":\"USER-SUB-1234\",\"noteId\":\"eb7d5540-bde9-11e9-851e-2b65657fd5ae\",\"content\":\"hello world\",\"attachment\":\"hello.jpg\",\"createdAt\":1565714798740}"
}

serverless invoke local --function create --path notes-app-api\mocks\create-event.json

Service Information
service: notes-app-api
stage: prod
region: us-east-1
stack: notes-app-api-prod
resources: 35
api keys:
None
endpoints:
POST - https://rn559aq7p0.execute-api.us-east-1.amazonaws.com/prod/notes
GET - https://rn559aq7p0.execute-api.us-east-1.amazonaws.com/prod/notes/{id}
GET - https://rn559aq7p0.execute-api.us-east-1.amazonaws.com/prod/notes
PUT - https://rn559aq7p0.execute-api.us-east-1.amazonaws.com/prod/notes/{id}
DELETE - https://rn559aq7p0.execute-api.us-east-1.amazonaws.com/prod/notes/{id}
functions:
create: notes-app-api-prod-create
get: notes-app-api-prod-get
list: notes-app-api-prod-list
update: notes-app-api-prod-update
delete: notes-app-api-prod-delete
layers:
None
Serverless: Run the "serverless" command to setup monitoring, troubleshooting and testing.

username pedro@taglivros.com.br
password Passw0rd!
user-pool-id us-east-1_u0WhuIEDY
app-client-id 30cvhbm2p8mvmmogpl2a9lkiir
cognito-region us-east-1
identity-pool-id us-east-1:b25e2bdc-9ea2-4e50-b7b6-1e5e9462cdc4
invoke-url https://ly55wbovq4.execute-api.us-east-1.amazonaws.com/prod
api-gateway-region us-east-1

npx aws-api-gateway-cli-test --username pedro@taglivros.com.br --password Passw0rd! --user-pool-id us-east-1_u0WhuIEDY --app-client-id 30cvhbm2p8mvmmogpl2a9lkiir --cognito-region us-east-1 --identity-pool-id us-east-1:b25e2bdc-9ea2-4e50-b7b6-1e5e9462cdc4 --invoke-url https://rn559aq7p0.execute-api.us-east-1.amazonaws.com/prod --api-gateway-region us-east-1 --path-template /notes --method POST --body "{\"content\":\"hello world\",\"attachment\":\"hello.jpg\"}"

Stopped
https://serverless-stack.com/chapters/create-a-login-page.html

confirm a user
aws cognito-idp admin-confirm-sign-up --region us-east-1 --user-pool-id us-east-1_u0WhuIEDY --username pedro.bnz@icloud.com
