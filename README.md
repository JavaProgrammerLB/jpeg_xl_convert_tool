# jpeg_xl_convert_tool
Convert 'view.jpg' to 'view.jxl' tool
![Xnip2025-01-09_17-31-17](https://github.com/user-attachments/assets/b5d853ed-74fb-4bae-9231-a9a0fde95bb3)

## How to Use

### 1. Fork this Repository
To fork this repository, follow these steps:
1. Navigate to the repository page on GitHub.
2. Click the "Fork" button in the upper right corner of the page.
3. Select your GitHub account to create the fork.

### 2 Create a GitHub Token
To create a GitHub token, follow these steps:
1. Go to GitHub and log in to your account.
2. Click on your profile picture in the upper right corner and select "Settings".
3. In the left sidebar, click on "Developer settings".
4. Click on "Personal access tokens" and then "Tokens (classic)".
5. Click the "Generate new token" button.
6. Fill in the "Note" field with a descriptive name for the token.
7. Select the scopes or permissions you need for the token.
8. Click the "Generate token" button.
9. Copy the generated token and save it in a secure place.

### 3 Set Up `WITH_GITHUB_TOKEN` Action Secret
To set up the `WITH_GITHUB_TOKEN` action secret in GitHub:
1. Go to the repository page on GitHub.
2. Click on the "Settings" tab.
3. In the left sidebar, click on "Secrets and variables" and then "Actions".
4. Click the "New repository secret" button.
5. Name the secret `WITH_GITHUB_TOKEN` and paste your GitHub token in the "Value" field.
6. Click "Add secret".

### 4. Modify and Push Image
To modify the image name and push it to GitHub:
1. Rename your JPEG image to `view.jpg`.
2. Place the `view.jpg` file in the `img` folder of the repository.
3. Commit and push the changes to your forked repository:
    ```sh
    git add img/view.jpg
    git commit -m "Add view.jpg to img folder"
    git push origin main
    ```

### 5. Create and Publish a Release
To create and publish a release on GitHub:
1. Go to the repository page on GitHub.
2. Click on the "Releases" tab.
3. Click the "Draft a new release" button.
4. Fill in the "Tag version" and "Release title" fields.
5. Click the "Publish release" button.

### 6. Wait for GitHub Action to Complete
After publishing the release, wait for the GitHub Action to complete. Once done, you will find the `jxl_file-${release_tag_name}.tar.gz` file containing the converted `.jxl` file on the release page created in step 4.
