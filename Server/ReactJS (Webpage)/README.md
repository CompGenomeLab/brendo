# Front-end

This folder includes the webpage content to be served to the end user. Importantly, it **does not** include the data itself, but webpage components. To run the full functionality, you will need to run the data server as well. If you are planning to serve Brendo through a server (eg. [nginx](https://nginx.org/)), the `build` folder generated here should go under some path such as `/var/www/<your-app-name>/`.

## Building
Run `yarn build`.

## Testing Locally
Run `yarn start`.
