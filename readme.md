# Here is some lib-crate readme

have some watermelon:

![watermelon.png](assets/watermelon.png)

# Steps to reproduce:

* check out 13d61c3de5ba834c1ae63a3af25e087e9b000dab (first commit)
* run `cargo doc --open`
* run `sh copy-assets-to-docs.sh` to copy the assets directories to target/docs so the html can reference them
* now, the generated docs have images as referenced in the markdown files.
* check out 61b1536245d56bfc9c7444cf4023bf7e8dcb71d9 (second commit)
* run `cargo doc --open`
* run `sh copy-assets-to-docs.sh` to copy the assets directories to target/docs so the html can reference them
* now, the generated docs even for the lib crate subdir have images as referenced in the markdown files.
* check out 7c91fe0034bd7d6691e1a5b20a4145568f902589 (third commit)
* run `cargo doc --open`
* run `sh copy-assets-to-docs.sh` to copy the assets directories to target/docs so the html can reference them
* now, the generated docs have an invalid link to an image in rustdoc-including-readmes-with-images/target/doc/binary/some_bin_module/index.html
