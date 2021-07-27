# How to use tailwind quickly

## Create dictory structure as following

```sh
mkdir test
cd test
npx tailwind init
touch t1.html t2.html
```

## Modify `tailwind.config.js`

Change from `purge: []` to `purge: ["./**/*.html"]`

## Generate `tail.css`

```sh
npx tailwind -o tail.css -m --jit
```

## Link `tail.css` to your html files

Now you can edit all your html files, then regenrate css file using above command.
Or run following command.

```sh
npx tailwind -o tail.css -m --jit -w
```
