# Sixth Sun - Unity Database Framework

This was a database framework used in the [Sixth Sun](https://bottomtextproductions.itch.io/the-sixth-sun) game project. This is a series of Unity Scriptable Objects that store values in a `Scene` and `GameObject` agnostic way. This implementation is based on the similar solution presented in the [*Unite Austin 2017 - Game Architecture With Scriptable Objects*](https://www.youtube.com/watch?v=raQ3iHhE_Kk) talk.

## Variable Types

This implementation supports types of data. All of the scriptable objects have `Dev Description` field that allows the designer to add a description to help them manage the database.

* **Numerical** values are stored as `float` and are returned in code as either `float` or `int`, depending on whether the designer chooses the `whole numbers` option in the editor. The scriptable object also supports clamping this variable between a min and max value.

    ![](Assets/Images/floatscreenshot.jpg)

* **Strings** 

    ![](Assets/Images/stringscreen.jpg)

* **Curves**. Stored as Unity's `AnimationCurve`
    
    ![](Assets/Images/curvescreen.jpg)

* **Keyboard Keys**. Using Unity's built-in `KeyCode` type, the variable stores and returns keyboard keys.

    ![](Assets/Images/keyscreen.jpg)

* **Vectors**. There are objects to store `Vector2` and `Vector3` values.

    ![](Assets/Images/vectortwoscreen.jpg)
    ![](Assets/Images/vector3screen.jpg)

## Usage

A Database Variable scriptable object can be created in the Asset browser of the Unity project by right-clicking and accessing the appropriate menu in `Create -> Game Variables` and then choosing the desired variable type.

## Third-Party Plugins

This implementation makes use of the following:
* [NaughtyAttributes](https://github.com/dbrizov/NaughtyAttributes) (MIT License)

## Credits

* [Rafael Castro e Silva](https://github.com/RafaelCS-Aula)
* [Hugo Feliciano](https://github.com/Xx-hugo-xX)