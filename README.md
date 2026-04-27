bookstore1
1-Middleware (Express): Função que executa entre a requisição e a resposta. O express.json() é essencial para ler dados JSON enviados por aplicativos mobile
2-NoSQL x SQL: SQL usa tabelas fixas e exige mudanças estruturais. NoSQL (como MongoDB) é mais flexível, ideal para catálogos de livros que mudam com frequência.
3-Hashing (bcryptjs): Converte senhas em códigos protegidos chamados hash. Se o banco vazar, as senhas reais não ficam expostas.
4-.env e dotenv: Guardam senhas, chaves e configurações fora do código. Isso aumenta a segurança e evita expor dados no GitHub ou em produção.

bookstore2
No signup, o usuário preenche username, email e password no app em React Native, que envia esses dados em JSON para o servidor. A API (ex: Express) valida as informações, verifica se o email já existe, criptografa a senha com bcryptjs e salva o novo usuário no MongoDB. Depois, retorna uma resposta de sucesso para o app, que pode redirecionar o usuário para login ou tela inicial.

