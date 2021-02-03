# Why does this exist?

This repo was created to host custom podspecs for Heir products to help speed up or enable compilation in iOS applications. This repo will most likely expand over time to include other internal dependencies.

The FirebaseFirestore podspec is copied from here: https://github.com/invertase/firestore-ios-sdk-frameworks/tree/7.3.0

The only reason why we have a custom fork of it is because of conflicts from the precompiled binaries provided by their pod and the Heircut iOS TensorFlowLiteC dependency. Our version has been edited to remove the conflicting dynamic_annotations symbol from the compiled binary thanks in to the guidance provided here: https://stackoverflow.com/questions/41217839/duplicate-symbols-when-integrating-firebase-and-google-sign-in-sdks-manually-wit