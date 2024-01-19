![Node.js Badge](https://img.shields.io/badge/node-%3E%3D%2012.0.0-brightgreen)
![npm Badge](https://img.shields.io/badge/npm-v6.14.4-blue)
![JavaScript Badge](https://img.shields.io/badge/language-JavaScript-yellow)
![Cheerio Badge](https://img.shields.io/badge/cheerio-v1.0.0-ff69b4)
![Express Badge](https://img.shields.io/badge/express-v4.17.1-lightgrey)
![Axios Badge](https://img.shields.io/badge/axios-v0.19.2-blueviolet)


# Climate Change News API

## Description
This Node.js application serves as a simple API to fetch climate change news articles from various online newspapers. 
The application uses `express` for setting up the server, `axios` for HTTP requests, and `cheerio` for parsing HTML content. 
The API scrapes specified news websites for articles containing the keyword "climate" and presents these articles in a JSON format.

## Features
- Fetches and displays a list of climate change related news articles.
- Allows filtering news articles by specific newspaper sources.
- Dynamically constructs article URLs from relative paths using base URLs.

## Installation

Before installation, ensure you have Node.js and npm installed on your system.

1. Clone the repository:
   ```sh
   git clone [repository-url]
   ```
2. Navigate to the project directory:
   ```sh
   cd [project-directory]
   ```
3. Install dependencies:
   ```sh
   npm install
   ```
### Commands to write the program from scratch on your local machine
```
node -v
npm init 
npm i cheerio
npm i express
npm i axios
npm i nodemon
npm run start
```

## Usage

Start the server with the following command:

```sh
npm run start
```

The server runs on `localhost` with the default port `8000` (configurable through environment variables).

### Endpoints

1. **Homepage (`/`):**
   - Returns a welcome message.
   - Method: `GET`

2. **All News (`/news`):**
   - Returns a JSON object with an array of all collected climate change news articles.
   - Method: `GET`

3. **News by Newspaper (`/news/:newspaperId`):**
   - Replace `:newspaperId` with the desired newspaper's name to get articles specifically from that source.
   - Method: `GET`

### Supported Newspapers

- CityAM
- The Times
- The Guardian
- The Telegraph
- New York Times
- Los Angeles Times
- Sydney Morning Herald
- BBC
- Evening Standard
- The Sun
- Daily Mail
- New York Post
- NASA
- CNN
- CBS News
- USA Today
- ABC News

## Configuration

The `newspapers` array in `index.js` contains the configuration for each newspaper source, including the name, base URL, and specific climate change section URL.

## Known Issues

- The link for 'UN News' is currently commented out due to issues causing API crashes.

## License

This project is licensed under the MIT License.


## Disclaimer

This API is for educational purposes only. The scraping functionality might be against the terms of service of the news websites. Always ensure compliance with legal guidelines and website terms when scraping data.


## Final Look 
![newspage.png](images%2Fnewspage.png)

![newspaperId.png](images%2FnewspaperId.png)
