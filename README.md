# UIUC Kappa Theta Tau main website
This is the documentation for Kappa Theta Tau's main website.

Table of contents
=
* [Cloning](#cloning)
* [Pushing Changes](#pushing-changes)
* [Updating Contacts](#updating-contacts)
* [Updating Brothers](#updating-brothers)
* [Development](#development)
	* [System Preparation](#system-preparation)
	* [Local Installation](#local-installation)
	* [Usage](#usage)
	* [Deploy](#deploy-with-gulp)

## Cloning
To clone this repo, simply git clone and cd into it.

```shell
$ git clone https://github.com/KappaThetaTau/kappathetatau.github.io.git & cd kappathetatai.github.io
```

## Pushing Changes
We are using github-pages to automatically compile and host our website. This means that to update the website, you simply need to push changes to your own branch and make a pull request on Github.

```shell
$ git checkout -b <new branch name>
...
<work on the website>
...
$ git add <whatever changes you made>
$ git commit -m "<meaningful commit message"
$ git push origin <new branch name>
<go make your pull request!>
```

## Updating Contacts
Contacts are managed by a CSV file located [here](_data/contacts.csv). To edit the contacts, simply edit this file

```shell
$ open _data/contacts.csv
```

## Updating Brothers
To update the [brothers](brothers.html) page we use a python [script](scripts/update_data.py) to pull the brother information and images from a google form CSV (https://goo.gl/forms/3MO7V2pyr4457p9h2).

```shell
$ python scripts/update_data.py
```

## Development
### System Preparation

1. [Jekyll](http://jekyllrb.com/) - `$ gem install jekyll`
2. [NodeJS](http://nodejs.org) - use the installer.
3. [GulpJS](https://github.com/gulpjs/gulp) - `$ npm install -g gulp` (mac users may need sudo)

### Local Installation
1. Clone this repo, or download it into a directory of your choice.
2. Inside the directory, run `npm install`.

### Usage
**development mode**

This will give you file watching, browser synchronisation, auto-rebuild, CSS injecting etc etc.

```shell
$ gulp
```

**jekyll**

As this is just a Jekyll project, you can use any of the commands listed in their [docs](http://jekyllrb.com/docs/usage/)

## Help!
Contact Dylan Huang at dylan.p.huang@gmail.com if you need any help updating or developing the website.
