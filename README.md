# z-Shell Setup

##### PLUGIN
`git` = default
`zsh-syntax-highlighting` = 코드가 변할 때 인식 시켜주는 plugin
`zsh-autosuggestions` = 다음에 입력할 코드를 예상해서 알려주는 plugin

```shell
	plugins=(
			git
			zsh-syntax-highlighting
			zsh-autosuggestions
			)
```


##### PC NAME REMOVE
```shell
	prompt_context() {
		if[[ "$USER" != "$DEFAULT_USER" || -n "$SSH_CLIENT" ]]; then
			prompt_segment black default "%(!.%{%F{yellow}%}.)$USER"
		fi
```
