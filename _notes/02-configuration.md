# Configurating Eleventy

## Create a configuration file

Create a `eleventy.config.js` file in the root of your project:

```js
export default async function (eleventyConfig) {
	return {
		dir: {
			input: "src",
			output: "_site",
		},
	};
}
```

This will make Markdown files in the `_notes` directory will not be processed by Eleventy.

## References

- [Configuration — Eleventy](https://www.11ty.dev/docs/config/)
