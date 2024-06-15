# Warm Challenge - picoCTF

## Challenge Description

This is a **picoCTF** challenge named "Warm." The objective of this challenge is to interact with a provided binary file to retrieve a flag. The flag is a string that is usually hidden within a program or system, and finding it requires understanding how to interact with the given resources.

## Challenge Type

This challenge falls under the category of **Binary Exploitation** or **Reverse Engineering**. It involves executing a binary file and understanding its behavior to extract hidden information, in this case, a flag.

## Steps to Solve

1. **Download the File:**

    The first step is to download the provided binary file from the given URL. This can be done using the `wget` command.

    ```sh
    wget https://mercury.picoctf.net/static/f95b1ee9f29d631d99073e34703a2826/warm
    ```

    This command downloads the file named `warm` from the specified URL.

2. **Make the File Executable:**

    Once the file is downloaded, it needs to be made executable. This is done using the `chmod` command with the `+x` flag, which grants execute permissions to the file.

    ```sh
    chmod +x warm
    ```

3. **Execute the File:**

    Run the file to understand its basic functionality. This is done by prefixing the filename with `./`, which tells the shell to execute the file in the current directory.

    ```sh
    ./warm
    ```

    The output of this command is:
    ```
    Hello user! Pass me a -h to learn what I can do!
    ```

    This indicates that the program supports a help flag (`-h`) to display more information.

4. **Run the File with the `-h` Flag:**

    To learn more about the file's functionality, run it with the `-h` flag.

    ```sh
    ./warm -h
    ```

    The output of this command is:
    ```
    Oh, help? I actually don't do much, but I do have this flag here: picoCTF{b1scu1ts_4nd_gr4vy_f0668f62}
    ```

    This output reveals the flag required to complete the challenge.

## Flag

The flag retrieved from the output of the program is:

`picoCTF{b1scu1ts_4nd_gr4vy_f0668f62}`


## Summary

This challenge required basic interaction with a binary file using common command-line tools. The primary steps included downloading the file, making it executable, and running it with appropriate flags to retrieve the flag. Understanding the usage of command-line arguments was crucial in solving this challenge.

## Tools Used

- `wget`: For downloading files from the internet.
- `chmod`: For changing file permissions to make the file executable.
- Shell (`bash`): For executing the commands.

## Learning Outcome

Participants learn to:
- Download and handle files from the command line.
- Modify file permissions to make them executable.
- Use help flags (`-h`) to explore the functionality of unknown programs.
