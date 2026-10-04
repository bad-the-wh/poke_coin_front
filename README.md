# 🪙 Poke Coin Frontend

The modern web user interface for the Poke Coin ecosystem, built with **Vue.js**. It provides a responsive, intuitive frontend dashboard for tracking assets, viewing real-time balances, and interacting with core application services.

---

## 🏗️ Project Architecture & Structure

The repository is structured following standard Vue CLI patterns:

```text
poke_coin_front/
├── public/                 # Static assets, HTML template, and favicons
├── src/                    # Source code (components, views, router, store/state)
├── .gitignore              # Git exclusion rules (node_modules, build outputs, etc.)
├── Dockerfile              # Container definition for production deployment
├── babel.config.js         # Babel transpiler configuration
├── jsconfig.json           # JavaScript project options and path alias settings
├── package.json            # Project dependencies and npm/yarn scripts
├── vue.config.js           # Vue CLI custom configuration overrides
└── yarn.lock               # Locked dependency versions
```

## 🛠️ Tech Stack

- **Framework: Vue.js (Composition/Options API architecture)

- **Language / Scripting: JavaScript, HTML5

- **Package Manager: Yarn

- **Build Tooling / Bundler: Vue CLI / Webpack

- **Containerization: Docker (Dockerfile)

## ⚙️ Getting Started & Local Development

#Prerequisites

Make sure you have Node.js (LTS recommended) and Yarn installed on your system.

#Installation & Scripts

- **Clone the repository:

```Bash
git clone [https://github.com/bad-the-wh/poke_coin_front.git](https://github.com/bad-the-wh/poke_coin_front.git)
cd poke_coin_front
```

- **Install dependencies:

```Bash
yarn install
```

- **Run the development server (with hot-reloading):

```Bash
yarn serve
```

The application will launch locally at http://localhost:8080.

- **Build for production:

```Bash
yarn build
```

Compiles and minifies files into the dist/ production bundle.

- **Lint and fix files:

```Bash
yarn lint
```

##🐳 Containerized Deployment
To build and run the frontend inside a Docker container:

```Bash
# Build the production image
docker build -t poke-coin-front .

# Run the container locally (mapping to port 80 or 8080 depending on your Nginx/server setup)
docker run -p 8080:80 poke-coin-front
```
