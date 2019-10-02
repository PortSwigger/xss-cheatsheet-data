This is the data that powers the [PortSwigger XSS cheat sheet](https://portswigger.net/web-security/cross-site-scripting/cheat-sheet). We have put this data on Github so the community can contribute vectors via pull requests.

## Contributing

To contribute please create a pull request with changes to the JSON data. 

For example, to add onwaiting to the data, do:

```javascript
"onwaiting": {
        "description": "Fires when while waiting for the data",
        "tags": [
            {
                "tag": "video",
                "code": "<video autoplay controls onwaiting=alert(1)><source src=\"validvideo.mp4\" type=video\/mp4><\/video>",
                "browsers": [
                    "edge"
                ],
                "interaction": false
            }
        ]
    }
```

The tags array contains the tags supported by the vector and browser support. Supported browsers are chrome,safari,firefox,edge all in lowercase. The interaction flag specifies if the vector requires user interaction.

Please make sure you search the data to ensure your vector hasn't already been added.
Please include your Twitter handle in the pull request message if you would like to be credited with it.

## License

The copyright for this project belongs to PortSwigger Web Security. We do not want this data to be used to create derivative cheat sheets hosted elsewhere, so we are not providing a license. That said, you are free to fork this repo in order to create pull requests back.
