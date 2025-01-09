# jpeg_xl_convert_tool
Convert 'view.jpg' to 'view.jxl' online tool

## How to Use

### 1. Fork this Repository
To fork this repository, follow these steps:
1. Navigate to the repository page on GitHub.
2. Click the "Fork" button in the upper right corner of the page.
3. Select your GitHub account to create the fork.

### 2. Set Up `WITH_GITHUB_TOKEN` Action Secret
To set up the `WITH_GITHUB_TOKEN` action secret in GitHub:
1. Go to the repository page on GitHub.
2. Click on the "Settings" tab.
3. In the left sidebar, click on "Secrets and variables" and then "Actions".
4. Click the "New repository secret" button.
5. Name the secret `WITH_GITHUB_TOKEN` and paste your GitHub token in the "Value" field.
6. Click "Add secret".

### 3. Modify and Push Image
To modify the image name and push it to GitHub:
1. Rename your JPEG image to `view.jpg`.
2. Place the `view.jpg` file in the `img` folder of the repository.
3. Commit and push the changes to your forked repository:
    ```sh
    git add img/view.jpg
    git commit -m "Add view.jpg to img folder"
    git push origin main
    ```

### 4. Create and Publish a Release
To create and publish a release on GitHub:
1. Go to the repository page on GitHub.
2. Click on the "Releases" tab.
3. Click the "Draft a new release" button.
4. Fill in the "Tag version" and "Release title" fields.
5. Click the "Publish release" button.

### 5. Wait for GitHub Action to Complete
After publishing the release, wait for the GitHub Action to complete. Once done, you will find the `jxl_file-${release_tag_name}.tar.gz` file containing the converted `.jxl` file on the release page created in step 4.