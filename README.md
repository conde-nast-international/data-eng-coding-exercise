# Data Engineer: Coding Exercise

This is a coding exercise to help us assess candidates looking to join the Data Engineering team at Condé Nast International.  The test is intended to be completed at home, and we expect you to spend no more than 1-2 hours on it.  If you don't have time to fully complete the exercise or you get stuck, that's fine and not entirely unexpected, just send us as much as you have done. We look forward to talking about your experiences.   

We understand that your time is valuable, and appreciate any time that you contribute towards building a strong team here.  If you really cannot spare the time, you may want to take a look at Option 2.

## Option 1

Implement a program that extracts the latest twenty five posts from https://www.facebook.com/BritishVogue, and writes to a csv file the id, message and number of shares for each of those posts.[1]

Your program should be designed such that it could be used in the future to collect all posts from hundreds of different facebook pages. As such, it should use a large scale data processing framework: we recommend [Apache Beam](https://beam.apache.org/) but you may choose another such as [Spark](https://spark.apache.org/) (using a local runner is fine).

You may implement in any language of your choice, and it is totally permitted to make use of any sample code, libraries or other resources available on the internet. Directly copying someone else's answer to this exact question is not advisable.

[1] if you are not familiar with the facebook api, you may use the [included response](facebook_api_response.json) which is what [the api](https://graph.facebook.com/v2.12/BritishVogue/feed?fields=message,id,shares) returned at time of writing. There's also a [version of the response](facebook_one_post_per_line.json) with one json object for each post per line, which may be easier to process.

And yes, we are aware that you could generate the output from the files provided with a simple [`jq`](https://stedolan.github.io/jq/) command ;)

## Option 2

If you have some personal code, or open source contribution, that you would be prepared to share with us, we can assess that instead.  The code should meet the following criteria:

- It should be at least 1-2 hours of your own work
- Ideally, it should involve an element of data processing
- It should demonstrate how you approach a problem
- It should be something that you are able to discuss with us

# Delivery

You can submit your code however you want - send the details to your point of contact.  Please include a README containing any setup instructions and keep the setup steps simple.

Please ensure you do not include any confidential information such as your facebook auth credentials.
