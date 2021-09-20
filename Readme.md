# Localhosting this site

### Step 1.
Download the [latest ruby installer](https://rubyinstaller.org/downloads/)

### Step 2.
Run the installer, when it presents you with 3 choices, execute them all in this order `1`, `2`, `3`

### Step 3. git clone this site

###

### Step 3.
Install the following gems via the CLI to install the needed gems;
```
$ bundle install
```

### Step 4.
Run the following commands in terminal;
```
$ bundle exec jekyll build

$ bundle exec jekyll serve
```
You should now be able to view the localhost @ http://localhost:4000/
Any file edits should regen on refresh