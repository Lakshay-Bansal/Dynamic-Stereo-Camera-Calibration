# Camera Model
The pinhole camera is as shown in Fig. 3.1. The light reflected from an object that needs to be captured passes through a pinhole and the image is formed on the
screen of the camera (inverted w.r.t. orientation of the object in the real world i.e. captured by camera). In the pin-hole camera model, it is assumed that all light
rays are passed through the pinhole’s center before being imaged on the screen. The pinhole camera model does not account for lens distortion because an ideal
pinhole camera does not have a lens. To accurately represent a real camera, the full camera model used by the algorithm of camera calibration includes radial and
tangential lens distortion. Usually, in the full camera model, only radial distortion is considered as shown in Fig. 3.2.


Fig. 3.1: Pin hole camera model
Source: https://in.mathworks.com/help/vision/ug/camera-calibration.html


Fig. 3.2: Radial distortion due to lens
Source: https://in.mathworks.com/help/vision/ug/camera-calibration.html



As shown in Fig. 3.3, the point P (Xw, Yw, Zw) in world coordinate is transformed to (Xc, Yc, Zc) from the reference frame of camera coordinate system by applying
rotation and translation to the world point (see Eq. 3.1). R (rotation matrix), is a 3 × 3 matrix and T (translation matrix) is a 3 × 1 matrix.

