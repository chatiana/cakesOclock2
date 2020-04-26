WebDevAppl - Cakes Oclock eCommerce
## Git
https://github.com/chatiana/cakesoclock2 

## Heroku
https://cakesoclock.herokuapp.com/

## Configuration
Platform: node v13.9.0,
Framework: express,
Database: mysql squelize,
Testing: ,
Deployment: heroku,
AWS: ECR, ECS, EC2, RDS,
app.js

        host: 'localhost',
        user: 'root',
        password : ******,
        port : 4300, 
        database:'cakesOclockSch'

## APIs are divided in three types

Users -
app.get('/register', registerjsfile.register);
app.post('/register_data', registerjsfile.register_data);
app.get('/login', registerjsfile.login);
app.post('/login_data',registerjsfile.login_data);
app.get('/logout', registerjsfile.loggout);
app.get('/profile', profilejsfile.profile);
app.get('/users', users.list);
app.get('/users/edit/:id', users.edit);
app.post('/users/edit/:id',users.save_edit);
app.get('/users/delete/:id', users.delete_user);


Products -
app.get('/products', products.list);
app.get('/items/:id', itemjsfile.items);
app.get('/adminproducts', adminproducts.list);
app.get('/adminproducts/add', adminproducts.add);
app.post('/adminproducts/add', adminproducts.save);
app.get('/adminproducts/edit/:id', adminproducts.edit);
app.post('/adminproducts/edit/:id',adminproducts.save_edit);
app.get('/adminproducts/delete/:id', adminproducts.delete_product);

Orders -
app.get('/adminorders', adminorders.list);

	
	


