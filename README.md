# Artist Of The Week

### Who Are You Listening To Right Now?
Checkout this week's [Spotify Playlist](https://open.spotify.com/user/gabejaquish/playlist/7lbtghXSJ6oatTVQyTBLOs?si=GOixKmkTQP-aGsyxeMKXWQ) or [Follow me on Spotify](https://open.spotify.com/user/gabejaquish?si=0ZzKz3B4SMGxdP5t1WwTow)

### History
Between 2005 and 2011 I ran a mobile DJ business, providing music, lighting, and announcements for Weddings, Retirements, Birthdays, county fairs, and all other manner of gathering. When you spend your weekends spinning (generally) the same hits over and over you tend to spend your weekdays searching for something different. Because let’s be honest, your wedding playlist isn't that original, most of it is probably songs from [Mobile Beat's Top 200 list](https://www.mobilebeat.com/top-200/), and that is totally fine. People love to dance to music they can sing along with.

In the winter of 2008 my brother introduced me to Spotify which materially changed the way I have consumed music, but it wasn't until 2015 that I realized the way I **listen** to music had changed. During my childhood up thru high school I tended to listen to Albums, start to finish, on Vinyl, 8-Track, CD, or even Digitally. Sure, DJing parties was song by song, but when I was home I liked to put on a record and sink into the album.

I work behind a desk, a lot of times alone, and a lot of times with headphones on, so in June of 2015 I decided to start a new tradition. Every Wednesday I would pick a new artist, read a bit about them, and Listen to all the albums and singles they had produced, start to finish, in chronological order. After I had listened to the artist's entire catalog, I would continue to listen to whatever songs or albums I liked best until the next Wednesday rolled around. Now I’m not going to claim this was a disciplined musical regimen each week. It wasn't and that wasn't the point. I would sometimes let myself wonder thru related artists, solo projects by band members, or even something different if I needed a break. 

It's a fun little journey thru the life of a particular band, artist or producer and gives you better insight into how they have changed and grown musically thru time, and I have stuck with it for 215 weeks as of this writing. 

### What is this repository for?
Given that I've been at this for a while, I thought it might be time to formalize some struture around my listening, and publish it online. Maybe even add some tracking who I am listening to each week. Maybe even record a little bit about each artist, like a fun fact, or a song I liked or disliked. Who knows.

Maybe someone else will find this idea interesting, or maybe I'll just be able to look back on who I liked best at a given period and see how my tastes have changed over time. 


### The Rules Of Engagement
1. "Artist Weeks" Begin on Wednesday and run to the following Tuesday. Wednesday morning begins a new Artist Week
1. The Artist Week should begin by listening to all recorded albums (live or studio) in cronological order, as released (not nessicarily recorded)
1. Once all albums have been listened to, you can listen to anything in the artist's catalog, collaborations, or songs they are featured on from other artists.
1. Weekends are free. Listen to whatever you want.


### How Are You Going To Record it?
Good Question, and I don't have a good answer. 

To start I am going to give JSON a try, recording the Artist's Name, Dates I listened, and a favorite song each week. I'll pull the new artist into the master each Wednesday and publish the file out to [my website](https://www.gabrieljaquish.com)


## Technical Stuffs
### JSON Standards
#### Dates
All dates will be formatted to comply with [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601). This simply means they are of the form YYYY-MM-DDD and will follow the Gregorian calendar.

#### The Format
* Conforms to most recent version of [JSON-Schema](http://json-schema.org/)
* Objects will be nested with the most recent week at the top
* Objects will be referenced (keyed) by the Wednesday on which they start
* Each Week Object will contain at minimum, but not be limited to, the following:
    * Date of Beginning Wednesday
    * Artist Name
    * Link to Spotify Artist Page
 * Optional Information Can Include
     * Favorite Song
     * Favorite Album
     * Wikipedia Link
     * Genre
     * Comments/Facts
  
 #### Example JSON   
 ```json
 {
	"2019-01-23": {
		"Artist": "khruangbin",
		"Spotify": "https://open.spotify.com/artist/2mVVjNmdjXZZDvhgQWiakk?si=Et3EKrg8SSK8Gio57HLhxA"
	},
	"2019-01-16": {
		"Artist": "The Marcus King Band",
		"Spotify": "https://open.spotify.com/artist/0tgaHqkU1p7QhBUIzKXVU9?si=9ps-yPFyTWyfG079oVKvcg"
	},
	"2019-01-09": {
		"Artist": "Colter Wall",
		"Spotify": "https://open.spotify.com/artist/3xYXYzm9H3RzyQgBrYwIcx?si=XD9EgIVmSxuRRNrgK7FimA",
		"Comment": "Colter is only 23, but has the sound of Johnny Cash meets Bob Dylan."
	}
}
```

## Contact

### Other Questions?
[Email Me](mailto:gabrieljaquish@gmail.com)


