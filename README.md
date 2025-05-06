# roadmap
Planning and researching the future of Goldentooth.

This will be split out into separate files soon...

- Finish up [Pulse](https://github.com/goldentooth/pulse/).
- Software/services in GitHub Profile README should go to repo topics or custom properties.
- Set up existing services to speak to Consul for service discovery. So we'll be able to e.g. see services announce themselves, see health checks, etc.
- Set up Authelia as a more secure front door. I would like to set up an account system eventually and grant privileges. Like, I don't _want_ people to destroy my cluster, not substantial privileges, but to be able to poke around a bit. Presumably read-only. See graphs, visualizations, etc.
- Tear down existing Nginx proxy. Nginx served its purpose but I'm fairly comfortable with it and I can use it in more interesting ways within the cluster. A couple of server blocks isn't that interesting. I wanna get weird with Nginx.
- Work on per-node pages, e.g. `https://node-name.goldentooth.net` that will show individual node status, logs, etc. Not sure what to do here yet -- currently they're static HTML. Might dynamically update them on a cron job. I could write a script that just gathers a bunch of figures, dumps them into JSON, and the HTML loads the JSON via JS and uses that to populate the page. Simple, clean, very flexible.
