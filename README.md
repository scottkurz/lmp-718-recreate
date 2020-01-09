# LMP-718-recreate
Recreate for https://github.com/OpenLiberty/ci.maven/issues/718

1. Clone project
```bash
git clone git@github.com:scottkurz/lmp-718-recreate.git; cd lmp-718-recreate
```

2. Create the server 
```bash
mvn liberty:create
```

3. Move intended server config into place
```bash
mv src/main/liberty/config/server.xml.moved  src/main/liberty/config/server.xml
```

4. Start dev mode (or run)
```bash
mvn liberty:dev    # or mvn liberty:run
```

5. Observe output:

> [INFO] [AUDIT   ] CWWKE0001I: The server defaultServer has been launched.  
> [INFO] [AUDIT   ] CWWKZ0058I: Monitoring dropins for applications.  
> [INFO] [ERROR   ] CWWKZ0013E: It is not possible to start two applications called starter-app.  
