# CodeBook

This is a code book that describes the variables, the data, and any transformations or work that you performed to clean up the data.

## The data source

* Original data: https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip
* Original description of the dataset: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

## Data Set Information

The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data.

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain.

## The data
Description of the DATA
The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. These time domain signals (prefix ‘t’ to denote time) were captured at a constant rate of 50 Hz. and the acceleration signal was then separated into body and gravity acceleration signals (tBodyAcc-XYZ and tGravityAcc-XYZ) – both using a low pass Butterworth filter.

The body linear acceleration and angular velocity were derived in time to obtain Jerk signals (tBodyAccJerk-XYZ and tBodyGyroJerk-XYZ). Also the magnitude of these three-dimensional signals were calculated using the Euclidean norm (tBodyAccMag, tGravityAccMag, tBodyAccJerkMag, tBodyGyroMag, tBodyGyroJerkMag).

A Fast Fourier Transform (FFT) was applied to some of these signals producing fBodyAcc-XYZ, fBodyAccJerk-XYZ, fBodyGyro-XYZ, fBodyAccJerkMag, fBodyGyroMag, fBodyGyroJerkMag. (Note the ‘f’ to indicate frequency domain signals).

Description of abbreviations of measurements

Body = related to body movement.
Gravity = acceleration of gravity
Acc = accelerometer measurement
Gyro = gyroscopic measurements
Jerk = sudden movement acceleration
Mag = magnitude of movement
mean and SD are calculated for each subject for each activity for each mean and SD measurements.
The units given are g’s for the accelerometer and rad/sec for the gyro and g/sec and rad/sec/sec for the corresponding jerks.

These signals were used to estimate variables of the feature vector for each pattern:
‘-XYZ’ is used to denote 3-axial signals in the X, Y and Z directions. They total 33 measurements including the 3 dimensions - the X,Y, and Z axes.

The tidy data set has been aggregated by Activity and Subject and return a mean value of each metric


The set of variables that were estimated from these signals are:
(For a description of the metrics please see the original datasets codebook)

Subject
Activity
TimeBodyAccelerometerMean()-X
TimeBodyAccelerometerMean()-Y
TimeBodyAccelerometerMean()-Z
TimeBodyAccelerometerSTD()-X
TimeBodyAccelerometerSTD()-Y
TimeBodyAccelerometerSTD()-Z
TimeGravityAccelerometerMean()-X
TimeGravityAccelerometerMean()-Y
TimeGravityAccelerometerMean()-Z
TimeGravityAccelerometerSTD()-X
TimeGravityAccelerometerSTD()-Y
TimeGravityAccelerometerSTD()-Z
TimeBodyAccelerometerJerkMean()-X
TimeBodyAccelerometerJerkMean()-Y
TimeBodyAccelerometerJerkMean()-Z
TimeBodyAccelerometerJerkSTD()-X
TimeBodyAccelerometerJerkSTD()-Y
TimeBodyAccelerometerJerkSTD()-Z
TimeBodyGyroscopeMean()-X
TimeBodyGyroscopeMean()-Y
TimeBodyGyroscopeMean()-Z
TimeBodyGyroscopeSTD()-X
TimeBodyGyroscopeSTD()-Y
TimeBodyGyroscopeSTD()-Z
TimeBodyGyroscopeJerkMean()-X
TimeBodyGyroscopeJerkMean()-Y
TimeBodyGyroscopeJerkMean()-Z
TimeBodyGyroscopeJerkSTD()-X
TimeBodyGyroscopeJerkSTD()-Y
TimeBodyGyroscopeJerkSTD()-Z
TimeBodyAccelerometerMagnitudeMean()
TimeBodyAccelerometerMagnitudeSTD()
TimeGravityAccelerometerMagnitudeMean()
TimeGravityAccelerometerMagnitudeSTD()
TimeBodyAccelerometerJerkMagnitudeMean()
TimeBodyAccelerometerJerkMagnitudeSTD()
TimeBodyGyroscopeMagnitudeMean()
TimeBodyGyroscopeMagnitudeSTD()
TimeBodyGyroscopeJerkMagnitudeMean()
TimeBodyGyroscopeJerkMagnitudeSTD()
FrequencyBodyAccelerometerMean()-X
FrequencyBodyAccelerometerMean()-Y
FrequencyBodyAccelerometerMean()-Z
FrequencyBodyAccelerometerSTD()-X
FrequencyBodyAccelerometerSTD()-Y
FrequencyBodyAccelerometerSTD()-Z
FrequencyBodyAccelerometerMeanFreq()-X
FrequencyBodyAccelerometerMeanFreq()-Y
FrequencyBodyAccelerometerMeanFreq()-Z
FrequencyBodyAccelerometerJerkMean()-X
FrequencyBodyAccelerometerJerkMean()-Y
FrequencyBodyAccelerometerJerkMean()-Z
FrequencyBodyAccelerometerJerkSTD()-X
FrequencyBodyAccelerometerJerkSTD()-Y
FrequencyBodyAccelerometerJerkSTD()-Z
FrequencyBodyAccelerometerJerkMeanFreq()-X
FrequencyBodyAccelerometerJerkMeanFreq()-Y
FrequencyBodyAccelerometerJerkMeanFreq()-Z
FrequencyBodyGyroscopeMean()-X
FrequencyBodyGyroscopeMean()-Y
FrequencyBodyGyroscopeMean()-Z
FrequencyBodyGyroscopeSTD()-X
FrequencyBodyGyroscopeSTD()-Y
FrequencyBodyGyroscopeSTD()-Z
FrequencyBodyGyroscopeMeanFreq()-X
FrequencyBodyGyroscopeMeanFreq()-Y
FrequencyBodyGyroscopeMeanFreq()-Z
FrequencyBodyAccelerometerMagnitudeMean()
FrequencyBodyAccelerometerMagnitudeSTD()
FrequencyBodyAccelerometerMagnitudeMeanFreq()
FrequencyBodyAccelerometerJerkMagnitudeMean()
FrequencyBodyAccelerometerJerkMagnitudeSTD()
FrequencyBodyAccelerometerJerkMagnitudeMeanFreq()
FrequencyBodyGyroscopeMagnitudeMean()
FrequencyBodyGyroscopeMagnitudeSTD()
FrequencyBodyGyroscopeMagnitudeMeanFreq()
FrequencyBodyGyroscopeJerkMagnitudeMean()
FrequencyBodyGyroscopeJerkMagnitudeSTD()
FrequencyBodyGyroscopeJerkMagnitudeMeanFreq()
Angle(TimeBodyAccelerometerMean,Gravity)
Angle(TimeBodyAccelerometerJerkMean),GravityMean)
Angle(TimeBodyGyroscopeMean,GravityMean)
Angle(TimeBodyGyroscopeJerkMean,GravityMean)
Angle(X,GravityMean)
Angle(Y,GravityMean)
Angle(Z,GravityMean)

