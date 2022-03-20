# SERVIDOR DENO CON HTTP SERVEST (run DENON)


### Install DENO
### `iwr https://deno.land/install.ps1 -useb | iex`
### Install DENON
### `deno install -qAf --unstable https://deno.land/x/denon/denon.ts`

### Configuracion para Visual Studio Code 
### `./.vscode/settings.json`
```json
{
    "deno.enable": true,
    "deno.suggest.imports.hosts": {
        "https://deno.land": true,
        "https://x.nest.land": true,
        "https://crux.land": true
    }   
}
```
### Run server 

`'denon run --allow-net ./server.tsx'`

```
PS E:\20610-programación-backend-20210906T233257Z-001\20610-programación-backend\Clase 47 - Deno_ el futuro de nodejs_\Desafio> denon run --allow-net .\servest.tsx
[*] [main] v2.5.0
[*] [daem] watching path(s): **/*.*
[*] [daem] watching extensions: ts,tsx,js,jsx,json
[!] [#0] starting `deno run --allow-net .\servest.tsx`
I[2022-03-20T03:44:59.533Z] servest:router listening on :8899
I[2022-03-20T03:45:05.759Z] servest:router 200 GET /
```
![](/011956.png)
```
[*] [daem] restarting due to changes...
[*] [daem] watching path(s): **/*.*
[*] [daem] watching extensions: ts,tsx,js,jsx,json
[!] [#0] starting `deno run --allow-net .\servest.tsx`
Check file:///E:/20610-programaci%C3%B3n-backend-20210906T233257Z-001/20610-programaci%C3%B3n-backend/Clase%2047%20-%20Deno_%20el%20futuro%20de%20nodejs_/Desafio/servest.tsx
I[2022-03-20T03:45:16.244Z] servest:router listening on :8080
I[2022-03-20T03:45:21.910Z] servest:router 200 GET /
I[2022-03-20T03:45:21.984Z] servest:router 404 GET /favicon.ico
```
![](/012115.png)