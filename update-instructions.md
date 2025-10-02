# Instructions for updating the website

### Making edits in code spaces
The easiest way to make edits is to use codespaces. Open the github repository, and click the green button that says "Code". There should be two options, one called "Local" and one called "Codespaces". Open up codespaces, and then click "Create codespace on main".

This should open up a code editor in your browser, where you can make edits to the files.


### Using Git
Whenever you make changes to the files in Codespaces, you will need to make sure that these changes are saved, commited, and pushed to github.

The workflow is the following:

1. Save your changes locally (e.g. ctrl + s on Windows, command + s on Mac).
2. Commit your changes on git. This makes sure that your local branch of git correctly registers the changes that you have made. There are two ways that you can do this:

    - First option: if you have only modified existing files and not created any new files, then you can commit your changes using the command:
        ```
        git commit -a -m "your message here"
        ```
    
    - Second option: if you have made new files that you want to be added to the github repository, then you need to add them and then commit them:
        ```
        git add --all

        git commit -m "your message here"
        ```
3. Once your changes have been commited, this only means that they have been registered on a local branch of Git, you also want to push them to the remote branch, which is what will actually deploy those changes to your website. The command to do this is:

    ```
    git push
    ```

There are lot's of online resources to brush up on the basic commands of git.


### File structure of repository
Because I was editing a template, the file structure of the repository is not necessarily the most intuitive. 

- `assets/media` contains all the pictures used in the website (e.g. the background, logo, etc.) 
- `config/_default` contains all the details about the config. This includes things like the seo and the headers/ footers for the website.
- `content/authors` contains all the details and information about group members. If you want to update this or add new members, you can do that here.
- `content/event` controls the information that appears in the "Activities" section of the website.
- `content/post` controls the information that appears in the "Projects" section of the website.
