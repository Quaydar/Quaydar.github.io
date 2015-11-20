---
published: false
title: Big 12 Geographic Expansion
layout: post
---
<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/1.0.2/Chart.min.js"></script>

A few years ago conference expansion was all the rage. To this day the Big 12 has been a constant conversation topic for conference expansion. Most certainly this is seen because of the CFP rankings and the possibility Big 12 teams get left out.

A lot of people like the idea of a geographic conference. I started looking at the number for teams that didn't belong in their conference (based purely on geographic concerns). The team that was the furthest away from their conference mates was Miami. That's a team that's rarely brought up as a location outlier.

However, Miami isn't the only "distant" team. Colorado, Maryland, Missouri, Nebraska, Texas A&M and West Virginia all moved to conferences where they'd be further away from their previous conference mates.

This leads to the idea of geographic expansion. Over time conferences tend to expand their regional footprint. This is easily represented by the Big 12 conference.

---

About methodology: all schools that play football in conference are included. The distances used are university to university (not stadium to stadium). The coordinates were entered and the distances are as the crow flies, calculated by a crude distance formula. Actual driving time and driving mileage will vary. Most of these shortcuts are to make the information manageable. If you don't like it, please do it better by querying the google maps API and share the results.

## Big 12 Average Distance Between Teams
<canvas id="big12" width="400" height="400"></canvas>


<script type="text/javascipt">
var data = {
   labels: [ "1996-2011", "2011-2012", "2012-present" ],
   datasets: [{
      label: "Average Distance",
fillColor: "rgba(220,220,220,0.2)",
            strokeColor: "rgba(220,220,220,1)",
            pointColor: "rgba(220,220,220,1)",
            pointStrokeColor: "#fff",
            pointHighlightFill: "#fff",
            pointHighlightStroke: "rgba(220,220,220,1)",
      data: [434,398,498]
   }]
};

var ctx = document.getElementById("big12").getContext("2d");
var myNewChart = new Chart(ctx).Line(data);
</script>
