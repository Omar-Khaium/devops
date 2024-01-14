# devops

## Step 1: Create a new repository on GitHub. To avoid errors, do not initialize the new repository with README, license, or gitignore files. You can add these files after your project has been pushed to GitHub.

```bash
git init
git add .
git commit -m "first commit"
git remote add origin <github-url>
git push -u origin master
```

## Step 2: Change the app name

- [ ] change the working branch to `change-app-name`

```bash
git checkout -b change-app-name
```

- [ ] add this package to pubspec.yaml

```yaml
dev_dependencies:
  change_app_package_name: any
```

- [ ] run this command

```bash
flutter pub get

flutter pub run change_app_package_name:main <new-app-name>
```

- [ ] commit and push

```bash
git add .
git commit -m "app name changed"
git push -u origin change-app-name
```