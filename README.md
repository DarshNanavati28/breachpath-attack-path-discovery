# BreachPath

BreachPath is a browser-based attack-path discovery tool for mapping identities, services, roles, permissions, trust relationships, and sensitive assets.

## Run locally

Open `index.html` in a modern browser. The app runs locally in the browser and does not upload model data.

## Model input

Build a model manually or import JSON. A model contains explicit `nodes` and directed `relationships`; every relationship endpoint must match a node ID. The app does not infer missing elements or links. Use the **JSON format** control in the app to download a starter file.

Supported element kinds: `user`, `service`, `role`, `permission`, and `asset`. Mark entry points and sensitive assets in the model builder. Paths are simple directed paths bounded by the selected maximum number of steps; loops are handled by skipping repeated elements.

## Deploy

This is a static site with `index.html` at the project root. It requires no build step; connect the repository to Vercel or deploy the folder as a static project.
