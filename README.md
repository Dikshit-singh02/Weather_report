

# Weather Fetcher Script

This is a simple Bash script that fetches the current weather for a given city using the `wttr.in` service.

## Prerequisites

Before running the script, make sure that you have the following installed on your Linux system:

- `curl` (the script uses `curl` to fetch weather data from the internet).
  
You can check if `curl` is installed by running:

    $ curl --version

If it's not installed, you can install it with the following command (on a Debian-based system):

    $ sudo apt-get install curl

## Usage

To use the script, simply run it from the command line with the name of the city as an argument.

### Example Usage:

    $ ./weather_fetcher.sh "New York"

This will return the current weather in the format:  
`Weather for New York: [condition]`

### Example Output:

    Fetching weather for New York...
    Weather in New York: 🌤 +18°C

You can also get more detailed weather information by running:

    $ curl wttr.in/New%20York

## Troubleshooting

- **Invalid City Name**: If the script does not return weather information for a city, ensure the city name is correct and try again.
  
- **curl errors**: If you encounter issues with the `curl` command (e.g., network problems), the script may not display the expected output. Check your internet connection or the `wttr.in` service's availability.

## Customization

- The format of the output can be customized by modifying the `wttr.in` URL. For example, to get more detailed information, change the `format=3` part of the URL. Refer to the [wttr.in documentation](https://github.com/chubin/wttr.in) for more options.

## License

This script is provided as-is. Feel free to modify and use it for personal purposes.

Explanation:

    Prerequisites: Informs the user that curl must be installed.
    Usage: Shows how to run the script and gives an example.
    Output: Describes what kind of output the user can expect when running the script.
    Troubleshooting: Offers solutions to common issues.
    Customization: Mentions how the script can be adjusted for different output formats via the wttr.in URL.
    License: A simple disclaimer about using and modifying the script.
