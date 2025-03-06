# CLI Tool Documentation

This document provides information on how to use our command-line interface (CLI) tool.

## Installation

To install the CLI tool, follow these steps:

1. Make sure you have Node.js installed on your system
2. Install the package globally using npm:



## Basic Usage

The CLI tool provides several commands to interact with the application from the command line:



## Available Commands

### greet

Greets a user with a customizable name.



If no name is provided, it defaults to "World".

**Example:**


### farewell

Bids farewell to a user with a customizable name.



If no name is provided, it defaults to "World".

**Example:**


### echo

Echoes a provided message.



The `--message` parameter is required for this command.

**Example:**


## Help

To display help information about the CLI tool and its commands:



## Options Reference

| Option | Description | Default | Required |
|--------|-------------|---------|----------|
| `--name <name>` | Specify the name for greet/farewell commands | "World" | No |
| `--message <msg>` | Specify the message for the echo command | - | Yes (for echo) |
| `--help` | Show help message | - | No |

## Error Handling

The CLI tool will exit with a non-zero status code in case of errors:

- If an unknown command is provided, it will display an error message, show the help information, and exit with status code 1.
- If the `echo` command is used without providing a message, it will display an error message and exit with status code 1.