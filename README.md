# Command Line Tools Buzz Session

Commands below assuming `debian:stretch`.

This repository includes a `Vagrant` profile that runs the included `Ansible` to setup a `Virtual Machine` with the tools discussed.

The following setup has been tested for the `Vagrant` host.

```
mocOS 10.13.6
Vagrant 2.1.2
VirtualBox 5.2.14 r123301
ansible 2.4.3.0
```

To start using the commands run the following:

```
vagrant up
vagrant ssh
```

## locate

Find files on your filesystem quickly using a portion of it's name.

```
locate <portion-of-filename>
```

Update the `locate` database.

```
sudo updatedb
```

Install with:

```
sudo apt-get install locate
```

## ncdu

Command line filesystem size utilisation with navigation.

```
cd <path>
ncdu
```

Install with:

```
sudo apt-get install ncdu
```

## tree

Directory tree listing.

```
cd <path>
tree
```

Install with:

```
sudo apt-get install tree
```

## pstree

Process tree listing.

```
pstree
```

Install with:

```
sudo apt-get install psmisc
```

## nmap

Network port scanner.

```
nmap <ip-or-domain-name>
```

Install with:

```
sudo apt-get install nmap
```

## lsof

Process owning an open file/port.

```
sudo lsof -i :<port>
```

Install with:

```
sudo apt-get install lsof
```

## mc

Midnight Commander command line file manager.

```
mc
```

Install with:

```
sudo apt-get install mc
```

## who

List currently logged in users.

```
who
```

## w

List currently logged in users and what they are doing.

```
w
```

## write

Send messages to another logged in user.

```
write <username> <tty>
```

## watch

Run a command repeatedly at a given interval.

```
watch <command>
```

## find

Find files in a give path.

```
find <path> -name "<file-name-expression>"
```

## cut

Remove line sections from a file.

```
cut -d'<delimiter>' -f <field-number> <filename>
```

## cd -

Return to the previous directory.

## pushd

Change to directory `<path>` and push current directory onto directory stack.

```
pushd <path>
```

## popd

Navigate to the directory at the top of the directory stack.

```
popd
```

## xargs

Execute command on standard out from previous command with `|`.

```
<command> | xargs <other-command>
```

## time

Time a command.

```
time <command>
```

## wondershaper

Network adapter shaping tool.

```
sudo wondershaper <adapter> <download> <upload>
```

Clear with:

```
sudo wondershaper remove <adapter>
```

Install with:

```
sudo apt-get install wondershaper
```

## jq

JSON processor.

```
jq
```

Install with:

```
<json> | jq '<filter>'
```
