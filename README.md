# Data Engineer: Coding Exercise

## The Exercise

Implement a program that extracts the latest ten posts from https://www.facebook.com/BritishVogue, and writes to a csv file the id, message and number of shares for each of those posts.[1]

Your program should be designed such that it could be used in the future to collect all posts from a large number different facebook pages. As such, it should use a big data processing framework: we recommend Apache Beam but you may choose another such as Spark. Using a local runner is fine.

You may implement in any language of your choice, and it is totally permitted to make use of any sample code, libraries or other resources available on the internet. Directly copying or being inspired by someone else's answer to this exact question is not advisable.

[1] if you are not familiar with the facebook api, you may use the [included response](facebook_api_response.json) which is what [the api](https://graph.facebook.com/v2.12/BritishVogue/feed?fields=message,id,shares) returned at time of writing. There's also a [version of the response](facebook_one_post_per_line.json) with one json object per line, which may be easier to process.

And yes, we are aware that you could generate the output from those files with a simple [`jq`](https://stedolan.github.io/jq/) command ;)

## Delivery

Supply the code to us either as a zip file, or a link to a public repository on GitHub. Please ensure you do not include any confidential information such as your facebook auth credentials. If you don't have time to fully complete the exercise or you get stuck, that's fine, just send us as much as you have done. We look forward to talking about your experiences.
