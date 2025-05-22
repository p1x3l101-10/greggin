A fork of the [GregTech Modern Community Pack](https://github.com/GregTechCEu/GregTech-Modern-Community-Pack), it is kept in sync with upstream using submodules, but I added my own stuff too

If you want to check my git hooks, they are located at [`autosign/hooks`](./autosign/hooks)

# How to install

Import the unsup Prismlauncher component into an empty instance on version `1.20.1` with forge installed (unsup can change the forge version, so dont worry about getting the correct version)
<details>
<summary>How to install a custom component</summary>
<br>
Create an empty component with the UID of <code>com.unascribed.unsup</code> with the following contents:
<pre><code>
{
  "formatVersion": 1,
  "name": "unsup",
  "uid": "com.unascribed.unsup",
  "version": "1.1.3",
  "+agents": [
    {
      "name": "com.unascribed:unsup:1.1.3",
      "url": "https://repo.sleeping.town"
    }
  ]
}
</code></pre>
You can save this component file for later by copying it from <code>&lt;INST_DIR&gt;/patches</code> to the central mods folder, then you can just click import component and select the component json.
</details>

And add the following java arguments:

```
-Dunsup.bootstrapUrl="https://raw.githubusercontent.com/p1x3l101-10/greggin/refs/heads/main/unsup.ini" -Dunsup.bootstrapKey="signify RWRBgYcfobPE7I7STPLaQnp69F06aqQaBSWk0AuUFKlUoCyE6VUZKxJv"
```

NOTE: Bootstrap URLs require unsup 1.1.3 or higher to use