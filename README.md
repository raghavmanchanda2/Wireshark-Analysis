# Wireshark Intro Analysis

## Overview
This project provides an analysis of network traffic using Wireshark, focusing on understanding protocols, packet transmission, and basic filtering techniques. The analysis includes examining HTTP requests and responses, identifying protocols, measuring transmission time, and applying display filters.

## Report
The detailed report containing the analysis of network traffic using Wireshark can be found in the file [Wireshark_Intro_Analysis_Report.pdf](Wireshark_Intro_Analysis_Report.pdf). Please refer to this document for in-depth insights and findings.

## Screenshots
For visual representations of the analysis, screenshots are provided in the [Screenshots](Screenshots) folder. Each screenshot corresponds to a specific section of the report.

- **Fig1.png**: Highlighted protocols in the unfiltered packet-listing window.
- **Fig2.png**: GET request arrival time.
- **Fig3.png**: HTTP OK arrival time.
- **Fig4.png**: Hyper Transfer Protocol information for OK response.
- **Fig5.png**: IP section of the GET request.
- **Fig6.png**: IP section of the OK response.
- **Fig7.png**: Transmission Control protocol information for the HTTP request.
- **Fig8.png**: Total packets captured and displayed, including IP address filtering.
- **Fig9.png**: Issue with IP address filtering.
- **Fig10.png**: Corrected IP address filtering.
- **Fig11.png**: Printed HTTP GET message.
- **Fig12.png**: Printed HTTP OK message.

## Usage
1. **Wireshark Installation**: Ensure Wireshark is installed on your system.
2. **Report Analysis**: Review the [Wireshark_Intro_Analysis_Report.pdf](Wireshark_Intro_Analysis_Report.pdf) for detailed analysis and findings.
3. **Screenshots**: Refer to the screenshots in the [Screenshots](Screenshots) folder for visual representations of the analysis.

## Contributing
Contributions are welcome. Please fork the repository, make your changes, and submit a pull request. For major changes, please open an issue first to discuss the proposed changes.

## Credits
- **Mr. RAGHAV MANCHANDA**: Author of the analysis report.

## License
This project is licensed under the [MIT License](LICENSE).


------------------------------------------------REPORT 2 BROWSER SERVER INTERACTION------------------------------------------------------

# Wireshark Browser Server Interaction Summary

## Overview
This document summarizes the analysis conducted on network traffic using Wireshark for Browser Server Interaction.

## Key Findings
1. **HTTP Versions**: Both the browser and the server are running HTTP 1.1 (see Fig 1 and Fig 2).
2. **Accepted Languages**: The browser indicates it can accept English (en-Gb, en-US) to the server (see Fig 3).
3. **Round-trip Time**: The round-trip time for the request is approximately 0.0305 seconds (see Fig 4).
4. **Status Code**: The server returns HTTP/1.1 200 OK status code to the browser (see Fig 5).
5. **Last Modified**: The HTML file was last modified on Fri, 23 Feb 2024 06:59:02 GMT (see Fig 6).
6. **Content Length**: The server returns 128 bytes of content to the browser (see Fig 7).
7. **Headers in Raw Data**: All headers are visible in the raw data without any missing headers (see Fig 8 and Fig 9).
8. **IF-MODIFIED-SINCE**: The first HTTP GET request does not include an “IF-MODIFIED-SINCE” line (see Fig 10), but it is present in the second request (see Fig 11).
9. **Server Response**: The server explicitly returns the contents of the file in the first HTTP GET response but not in the second, indicating that the file had not been modified (see Fig 12 and Fig 13).
10. **HTTP GET Messages**: Only one HTTP GET request message was sent by the browser (see Fig 17).
11. **HTTP Status Code**: Packet 32001 contains the status code HTTP/1.1 200 OK (see Fig 18).
12. **Data-containing TCP Segments**: Three TCP segments were needed to carry the single HTTP response (see Fig 20).
13. **TCP Overhead**: TCP overhead is calculated to be 1.21% of the entire TCP + HTTP + Data transmission (see Fig 21 and Fig 22).
14. **GET Requests and Addresses**: The browser sent 3 HTTP GET request messages to different Internet addresses (see Fig 23).
15. **Image Download**: The browser downloaded the two images serially rather than in parallel (see Fig 24 and Fig 25).

## Conclusion
This summary provides insights into the HTTP version, headers, status codes, round-trip time, and other aspects of network communication analyzed in Assignment using Wireshark.

This summary captures the key findings and insights from the report, providing a clear overview of the analysis conducted.
