# Aplicação de referência

Primeiro dia de trabalho e podemos conhecer a nossa **aplicação que está em desenvolvimento**.

É uma aplicação de backoffice com gestão de utilizadores, perfis, canais, etc..

![](images/screenshot_app_ref_001.png?raw=true)


### Pré-requisitos

* Conhecimentos de programação (independente de linguagem);
* Atuação na área de tecnologia;
* Preferencialmente Linux Ubuntu, embora possa usar Windows 10;
* Processador Quadcore com 8 Gb de RAM;

### Arquitetura da aplicação

![](images/arquitetura_aplicacao_referencia.PNG?raw=true)


### Setup

* Instalar java 8 ou superior
* Instalar NPM

### Executar a aplicação

**Backend**

```bash
> mvnw clean package
> mvnw spring-boot:run
```
```
[INFO] Scanning for projects...
[INFO]
[INFO] -------------------------< pt.its:backoffice >--------------------------
[INFO] Building backoffice 0.0.1-SNAPSHOT
[INFO] --------------------------------[ jar ]---------------------------------

...

2020-05-28 13:11:17.442  INFO 2687 --- [           main] o.s.s.concurrent.ThreadPoolTaskExecutor  : Initializing ExecutorService 'applicationTaskExecutor'
2020-05-28 13:11:17.765  INFO 2687 --- [           main] d.s.w.p.DocumentationPluginsBootstrapper : Context refreshed
2020-05-28 13:11:17.793  INFO 2687 --- [           main] d.s.w.p.DocumentationPluginsBootstrapper : Found 1 custom documentation plugin(s)
2020-05-28 13:11:17.839  INFO 2687 --- [           main] s.d.s.w.s.ApiListingReferenceScanner     : Scanning for api listing references
2020-05-28 13:11:18.037  INFO 2687 --- [           main] .d.s.w.r.o.CachingOperationNameGenerator : Generating unique operation named: findUsingGET_1
2020-05-28 13:11:18.097  INFO 2687 --- [           main] o.s.b.w.embedded.tomcat.TomcatWebServer  : Tomcat started on port(s): 8080 (http) with context path '/its-backoffice'
2020-05-28 13:11:18.099  INFO 2687 --- [           main] pt.its.backoffice.BackofficeApplication  : Started BackofficeApplication in 7.097 seconds (JVM running for 10.311)
```

**Frontend**
```
> npm install
...
> npm start
```
```
npm start

> backoffice-frontend@0.0.0 start K:\workspaces\default\backoffice-frontend
> ng serve

Browserslist: caniuse-lite is outdated. Please run next command `npm update`
10% building 3/3 modules 0 activei ｢wds｣: Project is running at http://localhost:4200/webpack-dev-server/
i ｢wds｣: webpack output is served from /
i ｢wds｣: 404s will fallback to //index.html

chunk {default~layout-login-login-module~user-user-module} default~layout-login-login-module~user-user-module.js, default~layout-login-login-module~user-user-module.js.map (default~layout-login-login-module~user-user-module) 32.6 kB  [rendered]
chunk {home-home-module} home-home-module.js, home-home-module.js.map (home-home-module) 6.56 kB  [rendered]
chunk {layout-layout-module} layout-layout-module.js, layout-layout-module.js.map (layout-layout-module) 35.1 kB  [rendered]
chunk {layout-login-login-module} layout-login-login-module.js, layout-login-login-module.js.map (layout-login-login-module) 54.8 kB  [rendered]
chunk {main} main.js, main.js.map (main) 52.2 kB [initial] [rendered]
chunk {polyfills} polyfills.js, polyfills.js.map (polyfills) 264 kB [initial] [rendered]
chunk {runtime} runtime.js, runtime.js.map (runtime) 9.24 kB [entry] [rendered]
chunk {scripts} scripts.js, scripts.js.map (scripts) 98.1 kB [entry] [rendered]
chunk {styles} styles.js, styles.js.map (styles) 2.37 MB [initial] [rendered]
chunk {user-user-module} user-user-module.js, user-user-module.js.map (user-user-module) 38.3 kB  [rendered]
chunk {vendor} vendor.js, vendor.js.map (vendor) 7.01 MB [initial] [rendered]
Date: 2020-05-28T12:10:51.923Z - Hash: 95e7b253dc74f320e85b - Time: 17855ms
** Angular Live Development Server is listening on localhost:4200, open your browser on http://localhost:4200/ **
i ｢wdm｣: Compiled successfully.
```

> Abrir no browser: **http://localhost:4200/**
