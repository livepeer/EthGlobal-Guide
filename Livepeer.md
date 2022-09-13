<Section name="1. Introduction" description="Introduction to Livepeer Ecosystem">

## What is the Livepeer Network

Livepeer is a decentralized video transcoding network that aims to enable cost effective, resilient, and censorship resistant video streaming, which today consumes 80% of internet bandwidth.

Through storytelling, illustration, and data, the [Livepeer Primer](https://livepeer.org/primer) explains, at a high level, the problem Livepeer solves, and how it works.

## What is Livepeer Studio

[Livepeer Studio](https://livepeer.studio/) provides all the tools needed to build web3 video apps with livestreaming, On Demand, and video NFT minting features.

<!-- <Quiz id={} />

### Question: What tool(s) does Livepeer Studio offer?
a. Live Streaming

b. Video On Demand

c. Video NFT minting

**d. All of the above** -->

</Section>

<Section name="2. On Demand" description="Introduction to On Demand Feature ">

## Uploading an Asset

> ⚠️ There are different ways to upload an asset (video & audio).

When uploading an asset using the API, there are two methods.

- Upload with URL (providing a downloadable URL)

- Upload with local storage (provide a `.mp4` file with H.264 video codec and AAC audio codec )

When using either the SDK or dashboard for uploading an asset, only providing a `.mp4` file with H.264 video codec and AAC audio codec is required.

<!-- <Quiz id={} />

### Question: T/F You can upload a video asset via the dashboard, sdk, or API?

TRUE -->

## Deleting an Asset

When deleting assets in Livepeer Studio, it can only be done through the API at the moment using the following endpoint:

- DELETE `/multistream/target/{id}` deletes an existing multistream target object. Make sure to remove any references to the target on existing streams before actually deleting it from the API.

- Response should return `204 No Content`

- Deleting an asset manually

<!-- <Quiz id={} />

**Question: T/F: You can delete an asset via the SDK or the dashboard.

FALSE,you can only upload an asset using the API at the moment. -->

## Updating an Asset

You can update the following attributes of an asset

1. asset name

2. storage

3. metadata for the video/audio asset

   - title

   - description

   - anything you want to customize

<!-- <Quiz id={} />

**QUESTION: T/F: You can update an existing video/audio file.**

FALSE, you can only update the name, storage and metadata for the asset. -->

</Section>

<Section name="3. Livestream" description="Introduction to Livestream Feature ">

## Starting a livestreaming

Log in to the Livepeer Studio Dashboard
Navigate to the [Streams page](https://www.livepeer.studio/dashboard/streams).

 On this page, you can create new streams and delete them. You can also click on a stream to find out details about the stream such as:

- Ingest URL

- Playback URL

- Health Metrics

- Stream Key

## Recording a livestreaming

  You can record a livestream either throught the dashboard, SDK or the API.

  >Recording livestreams will only work if it is enabled before the live stream starts.

- Multistreaming

Livepeer Studio has the ability to multistream by pushing the livestream to multiple ingest points of other targets such as Twitch, YouTube and many others.

- Video Playback

In order to playback a livestream with the playbackURL, a video player has to be used that supports HLS format. Livepeer Studio has a video player included in the SDK for video playabck, or the playbackURL can be passed in the Safari browser as it supports HLS natively.

>If wanting to only play the audio of livestream, just add `?video=false` at the end of the playbackURL.

<!-- <Quiz id={} />

**QUESTION: T/F: Can you paste a playback URL in the browser to view the stream?**

False, you need a video player in order to view the livestream in the borwser. The only exception is using the Safari browser as it supports HLS natively. -->

</Section>

<Section name="4. Minting Videos" description="Introduction to Mint NFT videos">

## Minting Video NFTs
Livepeer Studio has a step-by-step guide for minting video NFTs using the Video NFT SDK or creating your own transaction.

 🌿 [Minting Video Guide](https://docs.livepeer.studio/guides/mint-a-video-nft)

</Section>

<Section name="5. Using Livepeer Studio" description="Introduction Using Livepeer Studio">

## Using Livepeer Studio in your project

 🗝 [Create an API key](https://docs.livepeer.studio/quickstart)

 🖥 [Dashboard](https://livepeer.studio/dashboard)

🧰 [SDK](https://livepeerjs.org/)

 🛠 [API](https://docs.livepeer.studio/category/api)

</Section>

<Section name="Livepeer Studio Resources" description="Additional Resources">

## Livepeer Studio Resources

### [Quickstart](https://docs.livepeer.studio/quickstart)

Get an API key and start building with Livepeer Studio.

### [Stream via OBS](https://docs.livepeer.studio/guides/live/stream-via-obs)

Using [OBS](https://obsproject.com/) software for livestreaming.

### [In-browser Streaming](https://docs.livepeer.studio/guides/live/stream-from-the-browser)

Using Livepeer Studio's [WebRTMP SDK](https://github.com/livepeer/webrtmp-sdk) from in-browser livestreams.

### [Support Matrix](https://docs.livepeer.studio/reference/support-matrix)

Descriptions and highlights of some of Livepeer Studio's capabilities.

### [Example Applications](https://docs.livepeer.studio/reference/examples)

Example of applications that incorporated Livepeer Studio.

### [Discord](https://discord.gg/xVYJxEr3)

Join the Livepeer Studio Community

</Section>
