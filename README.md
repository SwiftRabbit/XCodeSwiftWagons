# XCodeSwiftWagons
Making wagons for the release train.

Instead of creating new targets, we share the target accross different schemes using a different build configuration.

New configurations can be created in the project info.
New schemes share the same target but use a different configuration.
The active compilation conditions (/ pragmas) are created inside the Build settings of the project for each configuration previously created.

All configuration share DEBUG.
All Active compilation flags are present in DEBUG (except for RELEASE).