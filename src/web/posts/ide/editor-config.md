# Configure Editorconfig

#### Sep 1, 2018 by Sreeram Padmanabhan

## Summary

This plugin attempts to override user/workspace settings with settings found in `.editorconfig` files. Below is my configuration.

## Install

Make sure you have installed the editorconfig extension for VS code.

## Configure

Create a file called `.editorconfig` at the root of the project with the following code.

## Code
    # http://editorconfig.org
    root = true

    [*]
    charset = utf-8
    end_of_line = lf
    indent_size = 2
    indent_style = space
    insert_final_newline = true
    max_line_length = 100
    trim_trailing_whitespace = true

    [*.md]
    max_line_length = 0
    trim_trailing_whitespace = false

    [COMMIT_EDITMSG]
    max_line_length = 0

Commit and push.