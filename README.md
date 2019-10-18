# SlimyCard - Animated Flutter Project

SlimyCard provides a beautiful slime-like animation of a Card that separates into two different Cards, one at the top and the another at bottom. It is possible to put any custom widget in these two separate cards.

![Banner Image](https://github.com/AkashDivya/SlimyCard-Animated-Flutter-Project/blob/master/images/SlimyCard-Animated-Flutter-Project-by-Akash-Divya.png)

# How to install this package

  - **1. Depend on it**

    Add this to your package's pubspec.yaml file:
    
    ```
    dependencies:
      slimy_card: ^1.0.0
    ```
    
  - **2. Install it**
    
    You can install packages from the command line:

    with Flutter:
    
    ```
    $ flutter pub get
    ```
    
    Alternatively, your editor might support flutter pub get. Check the docs for your editor to learn more.
    
# How to use this package

  - **1. Import it**
  
    In your Dart code, import the package as mentioned below:
    
    ```
    import 'package:slimy_card/slimy_card.dart';
    ```
    
  - **2. Use It**
  
    Create a ListView, and in its children use SlimyCard()
    
    ```
    ListView(
      children: <Widget>[
        SlimyCard(),
      ],
    );
    ```
    
  - **3. Custimize It**
    
    You can customize SlimyCard as per need, by using the following parameters:
    
    ```
    ListView(
      children: <Widget>[
        SlimyCard(
          color: Colors.red,
          width: 200,
          topCardHeight: 400,
          bottomCardHeight: 200,
          borderRadius: 15,
          topCardWidget: myWidget01(),
          bottomCardWidget: myWidget02(),
          slimeEnabled = true,
        ),
      ],
    ),
    ```
    
    **myWidget01** & **myWidget02** are your custom widget which you can display in Top Card & Bottom Card respectively.

# How to get the status of this package

  You can get the **real-time** status of this Package by wrapping the SlimeyCard in **StreamBuilder** as below:
  
  ```
  StreamBuilder(
    initialData: false,
    stream: slimyCard.stream, //Stream of SlimyCard
    builder: ((BuildContext context, AsyncSnapshot snapshot) {
      return ListView(
        children: <Widget>[
          SlimyCard(
            color: Colors.red,
            width: 200,
            topCardHeight: 400,
            bottomCardHeight: 200,
            borderRadius: 15,
            topCardWidget: myWidget01(),
            bottomCardWidget: myWidget02(),
            slimeEnabled = true,
          ),
        ],
      );
    }),
  ),
  ```
  
  snapshot.data will contain the **real-time**

# App Demonstration Video

  Cooming Soon...

# About Me

I'm a veteran Designer/Animator with **10+ years** of experience. I always hated the excuses Developers gave me when they fail to implement my Design. One day, when I found about Flutter I said no more & started learning it.

# Other Repo you may Like

[![Explore Flutter Firebase](https://raw.githubusercontent.com/AkashDivya/Explore-Flutter-FireStore/master/images/Banner.jpg)](https://github.com/AkashDivya/Explore-Flutter-FireStore)

[Visit this Repo](https://github.com/AkashDivya/Explore-Flutter-FireStore)

# My Links

**[Facebook](https://www.facebook.com/BadassDeveloperDesignerClub)**

**[YouTube](https://www.youtube.com/channel/UCo7mhMbZXaNgpyT7gM6mWDQ)**

**[Dribbble](https://www.dribbble.com/akashdivya)**

**[Behance](https://www.behance.net/akashdivya)**

**Email: akash.apd@gmail.com**

**Now go out there and do what you Love.**
