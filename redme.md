How to use:

Download the script and add it to a folder in your system PATH
Give it execution access (chmod +x update-android-project.sh)
Tweak the versions if needed
Run it from the root of your Flutter project









Looks good! But I would suggest to either change DESIRED_ANDROID_APPLICATION_VERSION name or add into a comment above information that this is Android Gradle Plugin (AGP) version. Also, instead of vague description for this variable This shouldn't be too old.. I would add a link to the official table of compatibility between Gradle version and Android Gradle Plugin versions: https://developer.android.com/build/releases/gradle-plugin

@alefwd
alefwd commented last week • 
about:

echo "Android project updated. Run 'git diff' to see the changes or 'git reset --hard' to discard them."
I would prefer 'git checkoout -- .' to clean up the temporary changes, instead of 'git reset --hard' which could cause problems by accident

@Asfemi
Asfemi commented last week
unable to get this to work, when i run the script nothing happens. smh