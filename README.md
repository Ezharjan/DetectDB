# [Sound Level Detector](https://ezharjan.github.io/DetectVolumn/)

A simple web interface is available for estimating the noise level in decibels. The values provided are not precise, but they primarily indicate variations in noise levels over a short period of time.

## Algorithm
The algorithm employed in this project involves calculating the noise level for different frequencies, calculating the average of those values, and then determining the average of all the values within a specific time interval known as the refresh rate (measured in milliseconds). The formula used to obtain a number approximation close to decibels is $20*log10(noiseValue)$, with an additional offset value added.

## Offset & Refresh Rate
To account for environmental noises and variations in microphone sensitivities, an adjustable offset value has been implemented. This offset value can increase or decrease the decibel measurements. By default, a value of 30 has been selected, as it has been found to produce the most satisfactory results. Additionally, the refresh rate for the decibel measurements can be adjusted, with a default setting of 1 second.

## Technnical Details
The web interface utilizes HTML5, CSS, and JavaScript. The JavaScript code responsible for estimating decibels is implemented using the Web Audio API, specifically the AudioContext Interface.

_[OriginalRepo](https://github.com/takispig/db-meter)_

<br>
<br>
<br>

*Slight Changes have been made in this repository.*
