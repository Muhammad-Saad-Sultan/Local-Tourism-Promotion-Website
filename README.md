# Local Tourism Promotion Website

This project is a static tourism website for promoting a selected region. It contains five interlinked HTML pages, a shared stylesheet, and a Parcel-based local build setup.

## Project structure

```text
campus-events/
├── .gitignore
├── .dockerignore
├── Dockerfile
├── package.json
├── README.md
├── src/
│   ├── index.html
│   ├── destination.html
│   ├── packages.html
│   ├── gallery.htm
│   └── contact.html
├── styles/
│   └── style.css
└── dist/
```

## Run locally

1. Open a terminal in `campus-events`.
2. Install dependencies:

```bash
npm install
```

3. Start the Parcel dev server:

```bash
npm start
```

4. Open the local URL shown in the terminal.

## Build for production

```bash
npm run build
```

The built site will be generated in `dist/`.

## Build Docker image

```bash
docker build -t your-dockerhub-username/campus-events:latest .
```

## Run Docker container

```bash
docker run -d -p 8080:80 your-dockerhub-username/campus-events:latest
```

Then open `http://localhost:8080`.

## Push to Docker Hub

1. Log in:

```bash
docker login
```

2. Push the image:

```bash
docker push your-dockerhub-username/campus-events:latest
```
