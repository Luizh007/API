### API
Criação de API(Application Programming Interface)
Primeiro, você precisa definir a rota da API que os usuários irão chamar. Por exemplo
                                    /api/users
                        
Depois tera que definir a função. Esta função irá lidar com a solicitação do usuário e retornar uma resposta. Por exemplo:
                                
                                function getUsers(req, res) {
                             const users = [ /* ... */ ];
                               res.send(users);
                                              }                 
                         
Agora crie um servidor você precisa criar um servidor web que irá ouvir as solicitações HTTP e chamar a função de manipulação de rota apropriada como mostra o exemplo:
                           
                          const express = require('express');
                          const app = express();

                          app.get('/api/users', getUsers);

                          app.listen(3000, () => {
                          console.log('API running on port 3000');
                           });
Este é apenas uns dos exemplos que existem simples de como criar uma API em JavaScript usando o framework Express.
Lembrado todos os arquivos javascript dentro das pastas ou subpastas automaticamente vão ser disponibilizadas como
rotas públicas
