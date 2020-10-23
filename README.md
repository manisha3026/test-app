# test-app
import 'package:flutter/material.dart';

void main() {
  runApp(MaterialApp(
    debugShowCheckedModeBanner: false,
    home: DefaultTabController(
      length: 3,
      child: Scaffold(
        appBar: AppBar(
          backgroundColor: Colors.blue,
          title: Text("Whatsapp",style: TextStyle(fontSize: 22.0,color: Colors.white),),
          actions: [
            Icon(Icons.search,size: 27.0,color:Colors.white),
            Icon(Icons.more_vert,size: 27.0,color: Colors.white,)
          ],
          bottom: TabBar(
            tabs: [
              //Tab(icon: Icon(Icons.camera_alt),),
              Tab(child: Text("Chats",style: TextStyle(color: Colors.white),),),
              Tab(child: Text("Status",style: TextStyle(color: Colors.white),),),
              Tab(child: Text("Calls",style: TextStyle(color: Colors.white),),),
            ],
          ),
        ),
        floatingActionButton: FloatingActionButton(
          backgroundColor: Colors.blue,
          child: Icon(Icons.message,size: 35.0,color: Colors.white,),
          onPressed: () {
            print("Floating button is pressed");
          },
        ),

      ),
    ),
  ));
}




