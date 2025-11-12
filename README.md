# alu-webstack https_ssl

## Project Overview

This project contains a Bash script named `0-world_wide_web` that audits DNS A records of specific subdomains for a given domain. It helps verify that subdomains like `www`, `lb-01`, `web-01`, and `web-02` point to the correct IP addresses.

## Script Usage

bash ./0-worldwideweb [subdomain]


- `<domain>`: The domain name to audit (mandatory).
- `[subdomain]`: Specific subdomain to audit (optional). If not provided, the script shows information for `www`, `lb-01`, `web-01`, and `web-02` subdomains in that order.

## Output Format

The script outputs lines in the following format:

The subdomain [SUBDOMAIN] is a [RECORD_TYPE] record and points to [DESTINATION]


## Requirements and Notes

- The script is written in Bash and uses `dig` and `awk`.
- It must be executed on Ubuntu 16.04 LTS.
- The script passes ShellCheck without errors.
- The script file is executable and starts with the proper shebang line.
- The project includes this README.md file at the root.

## Example

bash ./0-worldwideweb holberton.online
