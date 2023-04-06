### API
Criação de API(Application Programming Interface)
Primeiro, você precisa definir a rota da API que os usuários irão chamar. Por exemplo /api/users
                           
                           function getUsers(req, res) {
                             const users = [ /* ... */ ];
                               res.send(users);
                                              }
