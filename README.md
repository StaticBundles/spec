# StaticBundles

## What is StaticBundles

StaticBundles is a format for packaging static websites, which _bundles_ a
website's assets together with all the information needed by a server to host
the website.

To make a comparison, StaticBundles is for static websites what the OCI Image
Format is for server applications.

## What problem it tries to solve

You have a static website, like a Single-Page Application or a website built
with a static-site generator. The website consists of a bunch of files (html,
css, js, etc) in a directory. How do you deploy it?

The answer depends on the deployment platform you want to deploy to. Open Source
servers (NGINX, Apache, Caddy, etc), as well as commercial offerings (S3,
Netlify, Firebase Hosting, etc) each have their own way to make you deploy a
website.

This makes it difficult to switch between deployment platforms, locking you in
your chosen one, and also makes it difficult for the community to develop
tooling around the deployment process.

## How does it solve the problem

StaticBundles changes that, offering a deployment-platform-agnostic packaging
format, so that you only have to worry about packaging your website according to
the format, and you can then deploy it to any platform supporting the format.

To further the comparison above, once you package your server application into
an OCI Image, you can deploy said image to any deployment platofrm supporting
the format, like Kubernetes, AWS ECS, Heroku, etc.
