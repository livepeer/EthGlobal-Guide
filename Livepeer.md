# EthGlobal-Guide

<Section name="1. Introduction" description="Introduction to Livepeer Ecosystem">

## What is the Livepeer Network

Livepeer is a decentralized video transcoding network that aims to enable cost effective, resilient, and censorship resistant video streaming, which today consumes 80% of internet bandwidth.

Through storytelling, illustration, and data, the [Livepeer Primer](https://livepeer.org/primer) explains, at a high level, the problem Livepeer solves, and how it works.

## What is Livepeer Studio

[Livepeer Studio](https://livepeer.studio/) provides all the tools needed to build web3 video apps with livestreaming, video on demand, and video NFT minting features - web3 native, open infrastructure, affordable.

### Question: What tool(s) does Livepeer Studio offer?

<Quiz id={} />

a. Live Streaming

b. Video On Demand

c. Video NFT minting

**d. All of the above**

</Section>

<Section name="2. On Demand" description="Introduction to On Demand Feature ">

## Uploading an Asset

> ⚠️ There are different ways to upload an asset (video & audio).

- Using API

  - Upload with URL

  - Upload with locak storage

- Using SDK

  - Upload with local storage

- Using the dashboard

  - Upload with local storage

### Question: T/F You can upload a video asset via the dashboard, sdk, or API?

<Quiz id={} />


>TRUE

## Deleting an Asset

- Via the API

  - A DELETE Request

    - DELETE `/multistream/target/{id}` deletes an existing multistream target object. Make sure to remove any references to the target on existing streams before actually deleting it from the API.

    - Response should return `204 No Content`

- Via the Dashboard

  - Deleting an asset manually
**Question: T/F: You can delete an asset via the SDK or the dashboard.
<Quiz id={} />

>FALSE, you can only upload an asset using the API at the moment.

## Updating an Asset

You can update the following attributes of an asset

1. asset name

2. storage

3. metadata for the video/audio asset

   - title

   - description

   - anything you want to customize



<Quiz id={} />

**QUESTION: T/F: You can update an existing video/audio file.**

>FALSE, you can only update the name, storage and metadata for the asset.

</Section>
<Section name="3. Livestream" description="Introduction to Livestream Feature ">

- Starting a livestreaming

Log in to the Livepeer Studio Dashboard
Navigate to the Streams page, livepeer.studio/dashboard/streams. On this page, you can create a new stream and delete streams. When you name your stream, pick a unique name and include URL-compatible characters only.
On the Stream page (livepeer.studio/dashboard/streams), you can also click on a stream to find out configuration and usage information.

- Recording a livestreaming

  You can record a live stream either throught the dashboard, SDK or the API.

  >Recording livestreams will only work if it is enabled before the live stream starts.

- Multistreaming

Livepeer Studio has the ability to multistream by pushing the livestream to multiple ingest points of other targets such as Twitch, YouTube and many others.

- Video Playback

In order to playback a livestream with the playbackURL, a video player has to be used that supports HLS format. Livepeer Studio has a video player included in the SDK for video playabck, or the playbackURL can be passed in the Safari browser as it supports HLS natively.

If wanting to only play the audio of livestream, just add `?video=false` at thee 

</Section>


<Section name="4. Minting Videos" description="Introduction to Mint NFT videos">

[ ] [Minting Video Guide](https://docs.livepeer.studio/guides/mint-a-video-nft)

</Section>

<Section name="5. Using Livepeer Studio" description="Introduction Using Livepeer Studio">

## Using Livepeer Studio in your project

[ ] 🗝 [Create an API key](https://docs.livepeer.studio/quickstart)

[ ] 🖥 [Dashboard](https://livepeer.studio/dashboard)

[ ] 🧰 [SDK](https://livepeerjs.org/)

[ ] 🛠 [API](https://docs.livepeer.studio/category/api)

</Section>