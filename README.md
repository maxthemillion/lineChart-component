# d3 chart components

This repository contains chart components written in D3.js and Vue.js. Instead of re-writing the charts from scratch each time you build an interactive chart, use this one as a starting point and customize it when you require even more interactivity.

It comes with:
- data bindings to x-axis, y-axis and colors
- zooming
- panning
- annotation markers
- ...


## Installation [needs an update]
Install components using npm
> npm install @bit

Import to your main.js: 
> import app from '@maxthemillion/vued3-linechart'

## opts arguments [needs an update]
The opts object of the Linechart component takes the following arguments:
- dataURL: relative path to the data in csv format (eg. "./data/approval_allpolls.csv")
- chartTitle: string (eg. "How unpopular is Donald Trump?")
- chartSubTitle: string (eg. "Share of respondents disapproving the president (in %)")
- commentTitle: string that becomes the title for the chart's comment (eg. "The unwanted president")
- comment: string that explains the content of the chart in more detail
- binding: object with the following properties { 
    - x: heading of the data to map on the x-axis
    - y: heading of the data to map on the y-axis 
    - color: heading of the data to map to colors
    }
- xAxisTitle: string, null for no title
- yAxisTitle: string, null for no title
- colorScheme: d3-color scheme such as d3.schemeTableau10
- annotations: array of objects in the format {x: ... , text: ...}
