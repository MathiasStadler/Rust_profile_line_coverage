# project path

## Set project name
<!-- To comply with the format -->
```bash <!-- markdownlint-disable-line code-block-style -->
new_project_name="new_project"
# test
echo $new_project_name 
```
<!-- To comply with the format -->
## Create for your own project a project folder in the Linux console (terminal ,bash shell), e.g. in your your own home directory, and then open this folder as a new project in the MS VSCODE program
<!-- To comply with the format -->
```bash <!-- markdownlint-disable-line code-block-style -->
# cd && mkdir <new_project_name> folder && cd $_
# command 'cd' change to home folder from logged in user
# command `cd $_`change to create folder
cd && mkdir $new_project_name && cd $_
```
<!-- To comply with the format -->
!TODO Explain $_
!TODO Check inside a bash shell lastest version https://stackoverflow.com/questions/9450604/how-to-get-the-bash-version-number
<!-- To comply with the format -->
## Init a new rust based project inside the previously generated folder
<!-- To comply with the format -->
```bash <!-- markdownlint-disable-line code-block-style -->
touch README.md \
&& ln -s README.md README \
&& cargo init "." \
&& cargo add rustfmt \
&& rustup component add rustfmt \
&& mkdir examples \
&& cp src/main.rs examples/example.rs \
&& sed -i -e 's/world/example/g' examples/example.rs \
&& rustup  show \
&& rustup  check \
&& rustup toolchain uninstall stable \
&& rustup toolchain install stable \
&& rustup update  --force \
&& rustup show \
&& mkdir tests
```
!-- To comply with the format -->
>![!TIP]
>renew test folder
>`rm -rf test_folder/ && mkdir -p $_ && cd $_ && pwd &&   ls -la .
``
<!-- To comply with the format -->
## Init a new rust based project inside the previously generated folder for MS VSCode
<!-- To comply with the format -->
```bash <!-- markdownlint-disable-line code-block-style -->

mkdir -p .vscode \
&& touch .vscode/settings.json \
&& cat <<EOF > print.sh
#!/bin/bash
echo \$PWD
echo $PWD
EOF \
&& mkdir -p img \
&& wget  -P img/ "https://raw.githubusercontent.com/MathiasStadler/link_symbol_svg/360d1327d05280d53de5fa816c522f89a35891ca/img/link_symbol.svg" \
&& touch README.md \
&& ln -s README.md README \
&& cargo init "." \
&& cargo add rustfmt \
&& rustup component add rustfmt \
&& mkdir examples \
&& cp src/main.rs examples/example.rs \
&& sed -i -e 's/world/example/g' examples/example.rs \
&& rustup  show \
&& rustup  check \
&& rustup toolchain uninstall stable \
&& rustup toolchain install stable \
&& rustup update  --force \
&& rustup show \
&& mkdir tests
```