# piksep

Do you have a huge pile of photos of you and your friends and wish there existed some spell which would organize them according to who is there in the photos? Then piksep is what you are looking for! Just train it by feeding it some sample photos of your friends (so that piksep can learn how each of the persons look like!) before giving it the pile of unorganized photos.



## Installation

### Requirements

  * Python 2.7
  * macOS or Linux (Windows not officially supported, but might work)

### Prerequisites:

#### Installing prerequisites on Mac:

You will be needing a few libraries in order to run piksep. Install these libraries. Skip if you already have them. We will be using `brew` and `pip` to install them.

Install cmake using:
```bash
brew install cmake
```

Install boost using:
```bash
brew install boost
brew install boost-python --with-python3
```

Install numpy using:
```bash
pip install numpy
```

Install dlib using:
```bash
pip install dlib
```

Install click using:
```bash
pip install click
```

Install Pillow using:
```bash
pip install Pillow
```

#### Installing prerequisites on Linux:

#### Installing prerequisites on Windows:

### Getting piksep

Choose a folder where you want to keep piksep. Either download the entire code from [https://github.com/ankitshubham97/piksep](https://github.com/ankitshubham97/piksep) as zip file and unzip it or use ```git clone https://github.com/ankitshubham97/piksep.git```

## Using piksep

Open the root folder. You will see 2 folders: `input` and `unknown`.

<insert pic>
 
### Training photos

In the 'input' folder, you will put sample photos of all those people for whom you are going to run piksep. To do this, make separate folders for all the persons and name those folders after the names of the corresponding persons.

<insert pic>
 
Put not more than 2 or 3 sample photos in each of them (better if they have varying expressions :) ).

<insert pic>
 
Make sure that these photos do not have any other other faces too apart from the person intended. 

<insert pic>

This is for training piksep. It lets it learn what each of the persons look like.

### Unorganized photos

Put all the unorganized photos directly in the `unknown` folder. Note that all the photos must be 'directly' put in that folder, i.e. there should not be any folders in `unknown` folder.

<insert pic>

### Running piksep

Open a terminal in the root directory. Run piksep using the command 
```bash
python run.py
```

<insert pic>
 
It should start executing. You will see messages on the terminal reporting you about the execution process.

<insert pic>

### Getting the organized photos

In the end, you should see this message: `Find the folders in the 'output' folder.` It means that execution is over and you can find the organized pile at a newly created folder `output`.

<insert img>

Open the `output` folder and you will see different folders by the name of people for which you trained piksep for. You will find the photos of a particular person in the folder named after that person.

## Caveats

* It is definitely not 100% accurate.
* It does not work that well for children
* It does not work well if the person is wearing sunglasses

## Special mention

This project is forked from Adam Geitgey's repository [face_recognition](https://github.com/ageitgey/face_recognition). Visit that repository for a deeper insight of face ecognition mechanism!
