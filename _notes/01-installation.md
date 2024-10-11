# Setting up Eleventy

## Set up a new project

First, create a new directory and navigate to it:

```bash
mkdir eleventy-v3-webc
cd eleventy-v3-webc
```

Then, initialize a new npm project, and set the `type` of the project to `module`:

```bash
npm init -y
npm pkg set type="module"
```

now we have something like this in our `package.json`:

```json
{
	"name": "eleventy-v3-webc",
	"version": "1.0.0",
	"private": true,
	"type": "module",
	"scripts": {
		"test": "echo \"Error: no test specified\" && exit 1"
	},
	"author": "Masataka Yakura",
	"license": "ISC"
}
```

## Install Eleventy

Now, install Eleventy:

```bash
npm install @11ty/eleventy
```

Note: this project also uses [WebC](https://www.11ty.dev/docs/languages/webc/), but we're not ready for that yet. We'll install it later.

## Add convenient npm script commands

Right now, running Eleventy requires a bit long command:

```bash
npx @11ty/eleventy
```

Let's add a convenient npm script command to run Eleventy:

```json
{
	"scripts": {
		"dev": "eleventy --serve",
		"build": "eleventy",
		"eleventy": "eleventy"
	}
}
```

Now, you can run Eleventy with the following command:

```bash
npm run dev
```

yay.

## References

- [Getting Started — Eleventy](https://www.11ty.dev/docs/)
