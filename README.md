# MacOS Log Audit Tool

This log analysis script scans your macOS logs for specific patterns, which may indicate suspicious activity. It searches through the logs in the specified time range, identifies log entries matching the patterns, and writes the results to a file for further review.

## Features

- Detects various suspicious patterns in macOS logs.
- Multithreaded processing for faster log analysis.
- Configurable number of threads for optimal performance.
- Output file with timestamp for easy identification and review.

## Prerequisites

To use this script, you need:

- macOS system with logs to analyze.
- Bash shell (default shell in macOS).
`jq` installed.
`parralel` installed.

## Usage

Download the log analysis script and save it as log_analysis.sh:


# Download the script from the GitHub repository
` git clone https://github.com/hackerman-jpeg/MacOS_log_audit.git`

# Make the script executable
chmod +x log_analysis.sh

Run the script:
`./log_analysis.sh`

Follow the prompts to select the time range and the number of threads to use for log analysis.
The script will then process the logs and save the results in a file named audit_YYYY-MM-DD.txt.
Open the output file to review the results:

`open audit_YYYY-MM-DD.txt`
Replace YYYY-MM-DD with the current date.

## Customization

You can customize the script by modifying the patterns array to include additional log patterns to search for. For example:

```bash
patterns=(
  "failed to authenticate user"
  "new custom pattern"
)
```

## Contributing

I welcome contributions to improve this script. If you have ideas or suggestions, please submit an issue or a pull request on the GitHub repository.

## License

This script is open-source software, for more information, please see the LICENSE file.

## Disclaimer

This script is provided "as is" without any warranties or guarantees. Use it at your own risk. The author is not responsible for any damages or negative consequences arising from the use of this script.
