# Parsing methodology

The site I chose for parsing uses IP bans if it detects consequent automated requests. Simple measures, such as limiting the number of requests per second and faking user headers did not work, so more sophisticated approach was used - TOR. 

The basic use case for TOR  in my parser is changing the IP address every 10 seconds (that is the maximal frequency of IP updates). As a result, the target server is unable to detect the parser and lets me through. 

You can read more about various parsing approaches in the article written by me and [Philipp Ulyankin](https://github.com/FUlyankin) (currently only in Russian): https://habr.com/ru/company/ods/blog/346632/