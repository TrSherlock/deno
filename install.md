PowerShell (Windows) Kullan:
```batch
irm https://deno.land/install.ps1 | iex
```

index.ts
```tsx
import {Application} from './oak.ts'

const app = new Application();

app.use((ctx: any)=>{
    ctx.response.body='Hello World!';
});

await app.listen({port:8080})
```
oak.ts
```tsx
export { Application } from 'https://deno.land/x/oak/mod.ts';
```

Konsol
```batch
deno run --allow-net app.ts
```
