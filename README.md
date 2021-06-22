# Archiving-Linux-Data
### Scenario

 You will play the role of a security analyst for Credico Inc., a financial institution that offers checking, savings, and investment banking services.


- The company must comply with the Federal Trade Commission's Gramm-Leach-Bliley Act  which requires that financial institutions explain their information-sharing practices to their customers and protect sensitive data. 

#### Step 1: Create, Extract, Compress, and Manage tar Backup Archives

Creating `tar` archives is something you must do everyday in your role at Credico Inc. In this section, you will extract and exclude specific files and directories to help speed up your workflow.

To get started, navigate to the `~/Projects` directory where your downloaded `TarDocs.tar` archive file should be.

1. Extract the `TarDocs.tar` archive file into the current directory (`~/Projects`). Afterwards, list the directory's contents with `ls` to verify that you have extracted the archive properly.

      - Note that because we want to preserve the directory structure of our archive, we do not have to specify a target directory to extract to.

      - Note that when you run `ls` you should see a new `~/Projects/TarDocs` directory with five new subdirectories under `TarDocs/`.


Verify that there is a `Java` subdirectory in the `TarDocs/Documents` folder by running: `ls -l ~/Projects/TarDocs/Documents/`.

2. Create a `tar` archive called `Javaless_Docs.tar` that excludes the `Java` directory from the newly extracted `TarDocs/Document/` directory.

      - If you've executed this command properly, you should have a `Javaless_Docs.tar` archive in the `~/Projects` folder.

3. Verify that this new `Javaless_Docs.tar` archive does not contain the `Java` subdirectory by using `tar` to list the contents of `Javaless_Docs.tar` and then piping `grep` to search for `Java`.
