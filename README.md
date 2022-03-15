# Number-of-followers-from-YouTube
Number of followers from YouTube
$.ajax({

  type: 'GET',

  dataType: 'json',

  url: https://www.googleapis.com/youtube/v3/channels?part=statistics&id=YouTube_Channel_ID&key=API_key',

  success: function(data) {

    var ytcount = data.items[0].statistics.subscriberCount;

    $('.yt-count').html(ytcount);

  }

});
