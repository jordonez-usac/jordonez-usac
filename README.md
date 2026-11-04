<img src="https://capsule-render.vercel.app/api?type=waving&height=190&color=0:0b1220,55:1f4fbf,100:5ff3ff&text=Juan%20Ordo%C3%B1ez&fontColor=ffffff&fontSize=52&fontAlignY=34&desc=jordonez-usac&descSize=18&descAlignY=56&animation=fadeIn" width="100%" alt="Juan Ordoñez">

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&duration=2800&pause=900&color=4DA3FF&center=true&vCenter=true&width=640&lines=Estudiante+de+Ingenier%C3%ADa+en+Ciencias+y+Sistemas;Construyendo+KubeTrek%3A+Kubernetes+que+se+ve+en+vivo;Linux%2C+Go%2C+contenedores+e+IoT" alt="Estudiante de Ingeniería en Ciencias y Sistemas. Construyendo KubeTrek. Linux, Go, contenedores e IoT.">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Linux_Mint-22.3-3a7bff?style=flat-square&logo=linuxmint&logoColor=white" alt="Linux Mint 22.3">
  <img src="https://img.shields.io/badge/USAC-Guatemala-0b1220?style=flat-square" alt="USAC, Guatemala">
  <img src="https://komarev.com/ghpvc/?username=jordonez-usac&color=3a7bff&style=flat-square&label=visitas" alt="Visitas al perfil">
</p>

<p align="center">
  <img src="assets/neofetch.svg" width="780" alt="neofetch de juan@usac: Linux Mint, zsh, estudiante de Ingeniería en Ciencias y Sistemas en la USAC. Lenguajes: Go, JavaScript, Python, C++ y Java.">
</p>

## `~/proyectos/kubetrek`

<a href="https://github.com/kubetrek/kubetrek"><img src="assets/kubi.jpg" width="100%" alt="Kubi, el asistente de KubeTrek"></a>

<h3 align="center"><a href="https://github.com/kubetrek/kubetrek">KubeTrek</a></h3>

<p align="center">Aprende Kubernetes en tu propia terminal mientras la web te muestra en vivo lo que pasa en tu clúster.</p>

<p align="center">
  <a href="https://github.com/kubetrek/kubetrek"><img src="https://img.shields.io/badge/C%C3%B3digo-0b1220?style=for-the-badge&logo=github&logoColor=white" alt="Código"></a>
  <img src="https://img.shields.io/badge/Go-1.26-00ADD8?style=for-the-badge&logo=go&logoColor=white" alt="Go 1.26">
  <img src="https://img.shields.io/badge/Roadmap-3%2F8-3a7bff?style=for-the-badge" alt="Roadmap 3 de 8">
</p>

Kubernetes es difícil de aprender solo: escribes `kubectl apply`, recibes una línea de texto y todo lo demás pasa sin que lo veas. KubeTrek levanta un clúster real con kind en tu máquina, tú trabajas con `kubectl` de verdad, y la web dibuja cómo aparecen, cambian y mueren Deployments, ReplicaSets, Pods y Services. Cada paso se verifica solo, cada módulo termina con algo roto a propósito para que lo arregles, y Kubi te acompaña con pistas.

<details>
  <summary><b>Cómo funciona</b></summary>

```
 clúster kind  ◄─ watch ─  ktrek  ── WebSocket ──►  servidor  ── WebSocket ──►  navegador
 (tu máquina)                                       KubeTrek                   (grafo, pasos, Kubi)
```

`ktrek` vigila el namespace de la lección y manda los cambios a la web. Solo envía metadatos y estado, nunca el contenido de los Secrets ni los valores de las variables de entorno. La conexión sale de tu máquina, así que no hay que abrir puertos.

</details>

<details>
  <summary><b>Cómo se ve un módulo</b></summary>

**Pods y Deployments**

1. Aplica tu primer Deployment. ✓ 1 réplica lista
2. Borra un Pod y mira cómo aparece otro. ✓ el estado deseado en acción
3. Escala a 3. ✓ 3 réplicas listas
4. Despliega `nginx:1.27` y míralo en el grafo. ✓ todos los Pods con la imagen nueva
5. Regresa con `kubectl rollout undo`. ✓ revisión anterior

**Reto:** "Se desplegó una versión nueva y la app está caída. Arréglala."

</details>

<details>
  <summary><b>Ruta de aprendizaje</b></summary>

| Nivel | Temas |
|---|---|
| 1. Fundamentos | Arquitectura, Pods, Deployments, Services, ConfigMaps y Secrets |
| 2. Construir sobre Kubernetes (CKAD) | Probes, almacenamiento, Jobs, Ingress y Gateway API, Helm, Kustomize |
| 3. Operar el clúster (CKA) | Scheduling, RBAC, NetworkPolicies, autoescalado, backups de etcd |
| 4. Producción (SRE) | Prometheus, Grafana, Loki, Argo CD, Pod Security, operators |

</details>

<details>
  <summary><b>Roadmap</b></summary>

- [x] Experimentos técnicos (kind como librería, audit log, informers, consumo)
- [x] `ktrek up` / `ktrek down`, con apagado automático por inactividad
- [x] Agente que convierte los cambios del clúster en mensajes para la web
- [ ] Servidor relay y `ktrek connect`
- [ ] Grafo en vivo en el navegador
- [ ] Motor de módulos y los primeros módulos
- [ ] Cuentas con login de GitHub y progreso guardado
- [ ] Instaladores (Homebrew, script)

</details>

<p>
  <code>Go</code> <code>client-go</code> <code>kind</code> <code>Cobra</code> <code>WebSocket</code> <code>Kubernetes</code>
</p>

## `~/proyectos/smashgt`

<table>
  <tr>
    <td width="45%" valign="top">
      <a href="https://smashgt.pages.dev"><img src="assets/smashgt.jpg" alt="Portada de SmashGT"></a>
    </td>
    <td valign="top">
      <h3><a href="https://github.com/jordonez-usac/SmashGT">SmashGT</a></h3>
      <p>La escena competitiva de Super Smash Bros. Ultimate en Guatemala: ranking nacional, perfiles de jugadores, historial cara a cara y mapa de torneos por departamento.</p>
      <p><code>React</code> <code>Tailwind CSS</code> <code>Express</code> <code>MongoDB</code></p>
      <p>
        <a href="https://smashgt.pages.dev"><img src="https://img.shields.io/badge/Ver_el_sitio-3a7bff?style=for-the-badge&logo=cloudflarepages&logoColor=white" alt="Ver el sitio"></a>
        <a href="https://github.com/jordonez-usac/SmashGT"><img src="https://img.shields.io/badge/C%C3%B3digo-0b1220?style=for-the-badge&logo=github&logoColor=white" alt="Código"></a>
      </p>
    </td>
  </tr>
</table>

## `~/stack`

<table>
  <tr>
    <td><code>lenguajes</code></td>
    <td><img src="https://skillicons.dev/icons?i=go,js,python,cpp,java,bash" alt="Go, JavaScript, Python, C++, Java, Bash"></td>
  </tr>
  <tr>
    <td><code>web</code></td>
    <td><img src="https://skillicons.dev/icons?i=react,tailwind,vite,nodejs,express,mongodb" alt="React, Tailwind CSS, Vite, Node.js, Express, MongoDB"></td>
  </tr>
  <tr>
    <td><code>devops</code></td>
    <td><img src="https://skillicons.dev/icons?i=docker,kubernetes,linux,git,cloudflare" alt="Docker, Kubernetes, Linux, Git, Cloudflare"></td>
  </tr>
  <tr>
    <td><code>iot</code></td>
    <td><img src="https://skillicons.dev/icons?i=arduino,raspberrypi" alt="Arduino, Raspberry Pi">&nbsp;<img src="assets/mqtt.svg" width="48" alt="MQTT"></td>
  </tr>
</table>

## `~/actividad`

<p align="center">
  <img src="https://streak-stats.demolab.com?user=jordonez-usac&locale=es&background=0B1220&border=16213A&stroke=16213A&ring=3A7BFF&fire=5FF3FF&currStreakLabel=4DA3FF&sideLabels=D6DEEB&currStreakNum=FFFFFF&sideNums=FFFFFF&dates=6B7A99" alt="Racha de contribuciones">
</p>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/jordonez-usac/jordonez-usac/output/snake-dark.svg">
  <img src="https://raw.githubusercontent.com/jordonez-usac/jordonez-usac/output/snake.svg" width="100%" alt="Serpiente comiéndose el gráfico de contribuciones">
</picture>

<img src="https://capsule-render.vercel.app/api?type=waving&height=110&section=footer&color=0:0b1220,55:1f4fbf,100:5ff3ff" width="100%" alt="">
