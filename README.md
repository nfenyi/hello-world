/*
This file contains the attributes of my favorite song, Believe
and logs them to the console
 */
 
package com.example.introtokotlin

import androidx.appcompat.app.AppCompatActivity
import android.os.Bundle
import android.util.Log
import android.view.View

class MainActivity : AppCompatActivity() {
    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)
    }
//the name of the song
    val title : String = "Believe "
//the performer
    val artist : String = "Eminem"
//the composers of the song
    val songwriters = "Eminem, Mike Strange, Mark Baston, Luis Resto"
//the year the song was issued
    val yearReleased: Int = 2017
//style/category of music
    val genre :String= "Hip-hop/Rap"
//length of the song
    val duration :String = "5:15"
//name of set of recordings
    val album = "revival"
//owners of the song
    val copyright: String= "Universal Music Publishing Group, Kobalt Music Publishing Ltd., Me Gusta Music"
//number of  YouTube streams by November 2020
    val noOfStreams:Long= 7266802
//does the song have offensive or graphic content
    val isExplicit : Boolean = true
//position in album
    val trackNumber :Char = '2'
//this variable is declared and initialized just to prevent typing "MainActivity" repeatedly
    val tag = "MainActivity"

//this function logs the details of the song to the console when the button is tapped
    fun detais(view: View){

//this logs the title to the console
    Log.i("$tag", "Title: $title")
//this logs the artist to the console
    Log.i("$tag", "Artist: $artist")
//this logs the songwriters to the console
    Log.i("$tag", "Songwriters: $songwriters")
//this logs the year of release to the console
    Log.i("$tag", "Year of Release: $yearReleased")
//this logs the genre to the console
    Log.i("$tag", "Genre: $genre")
//this logs the duration of the song to the console
    Log.i("$tag", "Duration: $duration")
//this logs the name of its album to the console
    Log.i("$tag", "Album: $album")
//this logs the the copyrights to the console
    Log.i("$tag", "Copyrights: $copyright")
//this logs the number of streams to the console
    Log.i("$tag", "Number of YouTube streams: $noOfStreams")
//this logs the value of isExplicit to console
    Log.i("$tag","Is the song explicit?:$isExplicit")
//this logs the track number to the console
    Log.i("$tag","Track Number in Album:$trackNumber")
    }
}

