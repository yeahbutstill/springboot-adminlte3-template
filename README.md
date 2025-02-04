# springboot-adminlte3-template

### Things todo list:

1. Clone this repository: `git clone https://github.com/hendisantika/springboot-adminlte3-template.git`
2. Navigate to the folder: `cd springboot-adminlte3-template`
3. ```shell
    docker run --rm \
    --name=lte-db \
    -e MYSQL_DATABASE=lte \
    -e MYSQL_PASSWORD=root \
    -e MYSQL_ROOT_PASSWORD=root \
    -e TZ=Asia/Jakarta \
    -p 3306:3306 \
    -v "$PWD/docker/lte-db/conf.d":/etc/mysql/conf.d \
    -v "$PWD/storage/docker/ltedb-data":/var/lib/mysql \
    mysql:8
    ``` 
4. Run the application: `mvn clean spring-boot:run`
5. Open your favorite browser: http://localhost:8080

#### Images Screen shot

Register Page

![Register Page](img/register.png "Register Page")

Login Page

![Login Page](img/login.png "Login Page")

Dashboard Page

![Dashboard Page](img/dashboard.png "Dashboard Page")

Profile Page

![Profile Page](img/profile.png "Profile Page")

User List Page

![User List Page](img/user-list.png "User List Page")

User Add Page

![User Add Page](img/user-add.png "User Add Page")
