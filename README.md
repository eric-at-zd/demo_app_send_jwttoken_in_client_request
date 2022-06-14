# Test encoding and sending a JWT request to an external application

This app is an additional resource to the article [Encoding and Sending JSON web tokens](https://developer.zendesk.com/documentation/apps/app-developer-guide/using-the-apps-framework/#encoding-and-sending-json-web-tokens).

It demonstrates the following:

- Using `client.metadata` to load parameters for use in your application
- Using `client.request` to encode and send a JWT request to an external server
- Using [Custom Claims](https://auth0.com/docs/secure/tokens/json-web-tokens/json-web-token-claims) for your unique JWT workflows

When running, bring up your browser's Console tab and Network tab to monitor the different behaviors.

## Getting started

This app needs a web server for us to be able to pass the JWT request to. You can create your own copy of our example by clicking [here](https://glitch.com/edit/#!/remix/defiant-caring-chestnut). Take note of the name / url (available from the share button in the upper right hand corner) of the web server as you'll need this in the future steps.

Follow these steps to get a local copy of your Zendesk app up and running.

### Prerequisites

- Zendesk Command Line (ZCLI)

[Using Zendesk Command Line](https://developer.zendesk.com/documentation/apps/app-developer-guide/zcli/#installing-and-updating-zcli)

### Installation

1. Clone the repo.

   ```bash
   git clone https://github.com/example.git
   ```

2. Navigate into the directory.

   ```bash
   cd demo_app_send_jwttoken_in_client_request
   ```

3. [Install the app](https://developer.zendesk.com/documentation/apps/app-developer-guide/zcli/#packaging-and-installing-a-private-zendesk-app).

   ```bash
   zcli apps:create .
   ```

4. Once the app has been installed, you'll be asked for the serverUrl. Input the glitch url from the previous steps.

[Packaging and installing a private Zendesk app]()

<!-- Links to relevant resources such as help center articles or dev docs -->

## Additional Resources

- [How ZAF client.request works](https://developer.zendesk.com/documentation/apps/getting-started/how-apps-framework-client-request-works/)
- [Zendesk Apps Guide](https://developer.zendesk.com/documentation/apps/)
- [Apps Support API documentation](https://developer.zendesk.com/api-reference/apps/apps-support-api/introduction/)
- [MDN web docs for the Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)
- [ZAF notify method](https://developer.zendesk.com/api-reference/apps/apps-support-api/all_locations/#notify)

<!-- Issue reporting with link to repo issues page -->

## Issues

You can [create an issue on Github](https://github.com/zendesk/example/issues/new),
reach out in our [Developer Community](https://support.zendesk.com/hc/en-us/community/topics),
or report the issue in the [Zendesk Developers Slack group](https://docs.google.com/forms/d/e/1FAIpQLScm_rDLWwzWnq6PpYWFOR_PwMaSBcaFft-1pYornQtBGAaiJA/viewform).
