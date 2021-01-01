# jekyll-builder

I don't want to install ruby, so I am using docker to allow me to create jekyll projects without installing ruby

## Usage

Build a new Jekyll project:

```bash
docker build -t jekyll .
docker run -d --name builder jekyll new <project-name>
docker cp builder:/<project-name> <path-on-host>
```
