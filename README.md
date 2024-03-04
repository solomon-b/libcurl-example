```bash
➜ gcc http-post.c                                                                  
/nix/store/3z013mdl9cvpgvavpj19rbilihz4clvi-binutils-2.40/bin/ld: /tmp/ccUqv7fq.o: in function `main':
http-post.c:(.text.startup+0x7): undefined reference to `curl_global_init'
/nix/store/3z013mdl9cvpgvavpj19rbilihz4clvi-binutils-2.40/bin/ld: http-post.c:(.text.startup+0xc): undefined reference to `curl_easy_init'
/nix/store/3z013mdl9cvpgvavpj19rbilihz4clvi-binutils-2.40/bin/ld: http-post.c:(.text.startup+0x26): undefined reference to `curl_slist_append'
/nix/store/3z013mdl9cvpgvavpj19rbilihz4clvi-binutils-2.40/bin/ld: http-post.c:(.text.startup+0x35): undefined reference to `curl_slist_append'
/nix/store/3z013mdl9cvpgvavpj19rbilihz4clvi-binutils-2.40/bin/ld: http-post.c:(.text.startup+0x44): undefined reference to `curl_slist_append'
/nix/store/3z013mdl9cvpgvavpj19rbilihz4clvi-binutils-2.40/bin/ld: http-post.c:(.text.startup+0x53): undefined reference to `curl_slist_append'
/nix/store/3z013mdl9cvpgvavpj19rbilihz4clvi-binutils-2.40/bin/ld: http-post.c:(.text.startup+0x65): undefined reference to `curl_easy_setopt'
/nix/store/3z013mdl9cvpgvavpj19rbilihz4clvi-binutils-2.40/bin/ld: http-post.c:(.text.startup+0x7b): undefined reference to `curl_easy_setopt'
/nix/store/3z013mdl9cvpgvavpj19rbilihz4clvi-binutils-2.40/bin/ld: http-post.c:(.text.startup+0x91): undefined reference to `curl_easy_setopt'
/nix/store/3z013mdl9cvpgvavpj19rbilihz4clvi-binutils-2.40/bin/ld: http-post.c:(.text.startup+0x99): undefined reference to `curl_easy_perform'
/nix/store/3z013mdl9cvpgvavpj19rbilihz4clvi-binutils-2.40/bin/ld: http-post.c:(.text.startup+0xa5): undefined reference to `curl_easy_cleanup'
/nix/store/3z013mdl9cvpgvavpj19rbilihz4clvi-binutils-2.40/bin/ld: http-post.c:(.text.startup+0xaa): undefined reference to `curl_global_cleanup'
/nix/store/3z013mdl9cvpgvavpj19rbilihz4clvi-binutils-2.40/bin/ld: http-post.c:(.text.startup+0xb5): undefined reference to `curl_easy_strerror'
collect2: error: ld returned 1 exit status
```

```bash
➜ gcc http-post.c -lcurl

```
