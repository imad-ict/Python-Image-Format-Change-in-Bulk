import os
import cv2

def changeFormat(folder, format):
    '''

    :param folder: folder path
    :param format: format to change to.
    :return:
    '''
    l1 = os.listdir(folder)
    for i in l1:
        img = cv2.imread(os.path.join(folder, i))
        cv2.imwrite(os.path.join(folder, i), img, [int(cv2.IMWRITE_JPEG_QUALITY), 100])

if __name__ == "__main__":
    folder = "data/images/train"
    changeFormat(folder, "png")
