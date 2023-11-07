website deploy: https://luxury-tanuki-7c3787.netlify.app/

# Quarto deploy day 1

Able to deploy without docs folder

When trying to remove freeze folder ran into error

Tried to add build command in netlify.toml but error was not resolve

```
[build.environment]
  environment = { R_VERSION = "4.1.1" }
[[plugins]]
package = "@quarto/netlify-plugin-quarto"
```

Error from netlify when removed \_freeze folder

![screenshot](/Screenshot%202023-11-07%20at%2011.06.54 AM.png)

Leighton and I decided to colab and worked on merge conflict

when we set
`freeze:false` in the quarto.yml it seems like there is no conflict

without it we have a minor conflict with hash but it was resolved easily

# Next steps

I wanted to test if multiple people commit at the same time would there be more major conflict or just those minor one that we have tested
