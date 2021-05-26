# coder-home-dir

In Coder on Kubernetes, an image's `/home/<user>` directory is not used, as it is replaced by a Persistant Volume Claim so that the developer doesn't loose their files on rebuilds. Everything else in the filesystem is ephemeral and relies on the image as a source-of-truth. [See the docs](https://coder.com/docs/workspaces/personalization#persistent-home)

This is an example project that copies over an initial home directory from another folder. [See video](https://kapwi.ng/c/UkP3xaVA)

See the [.coder/](.coder/) folder for a sample image and corresponding template to copy the initial files.

An individual developer can also further customize their home directory with a [dotfiles repo or a personalize script](https://coder.com/docs/workspaces/personalization).
