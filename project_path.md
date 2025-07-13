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
cd && mkdir $new_project_name && cd $_ && pwd
```
<!-- To comply with the format -->
TODO Explain $_
TODO Check inside a bash shell lastest version
TODO https://stackoverflow.com/questions/9450604/how-to-get-the-bash-version-number
FIXME
XXX
BUG
HACK,
FIXME,
TODO
XXX
[ ]
[x]
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
<!-- To comply with the format -->
>[!TIP]
>Markdown inline code block - https://markdown.land/markdown-code-block
#FIXIT Link :-)
>Use `print("Hello, world!")` to print a message to the screen.
<!-- To comply with the format -->
>[!TIP]
>Managing Spaces in Markdown - &nbsp;
FIXIT https://www.markdowntoolbox.com/blog/spaces-in-markdown/
>[!TIP]
>Renew test folder&nbsp;&nbsp;
>`rm -rf test_folder/ || true && mkdir -p $_ && cd $_ && pwd &&   ls -la .`
>> `|| true `works if the file/directory does not exist and does not throw an error
>Renew current folder
>`_current_folder=$(pwd) && echo $_current_folder && rm -rf _current_folder/ || true && mkdir -p $_ && cd $_ && pwd &&   ls -la .`
<!-- To comply with the format -->
## Create a new Rust-based project within the previously generated folder for use in the MS VSCode tool
<!-- To comply with the format -->
- Use a standard Bash shell without extensions such as AI/Copilot, etc
<!-- To comply with the format -->
```bash <!-- markdownlint-disable-line code-block-style -->
mkdir -p .vscode \
&& touch .vscode/settings.json \
&& cat <<EoF >.vscode/settings.json
{
    "cSpell.words": [
        "binutils",
        "ccache",
        "debuginfo",
        "euxo",
        "evcxr",
        "FIXIT",
        "grcov",
        "nextest",
        "objcopy",
        "objdump",
        "pipefail",
        "profdata",
        "readobj",
        "rustfilt",
        "rustup",
        "sccache"
    ]
}
EoF \
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

TODO Explain $_
TODO Check inside a bash shell lastest version
TODO https://stackoverflow.com/questions/9450604/how-to-get-the-bash-version-number
FIXME
XXX
BUG
HACK,
FIXME,
TODO
XXX
[ ]
[x]