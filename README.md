## caMicroscope GSoC 2020
caMicroscope is a digital pathology image viewer with support for human/machine generated annotations and markups. The source code of the caMicroscope project can be found at https://github.com/camicroscope/caMicroscope, released with BSD 3-Clause License. In addition to the caMicroscope project, caMicroscope as an organization also hosts several related tools and products at https://github.com/camicroscope/

This is the first year that caMicroscope plans to participate in GSoC as a mentoring organization. However, we have been an open source organization for 7 years since inception. Our GSoC mentoring team is composed of past GSoC organization administrators, mentors, and students from the other organizations that participated in the GSoC in the previous years.

Communicating with the mentors
We intend to use Slack as the primary medium of communication. The slack room at camicroscope.slack.com is used to discuss project ideas. You may join the caMicroscope Slack channel through our shared link - http://bit.ly/camicroscope

List of Ideas
The following ideas were created with feedback from contributors and collaborators. Submissions need not come from the below list, but should have reasonable relevance to the caMicroscope organization and its goals. Please feel free to discuss these or other project ideas on the email list or Slack group.

[1] Cancer Region of Interest Extraction and Machine Learning

Mentors: Insiyah Hajoori and Ryan Birmingham

Overview:

This project would involve extending the existing machine learning intergrations beyond marking up images, and allow users to fetch regions of interest from a given slide automatically. This would allow for users and scientists to train other models for tasks such as synthetic data generation. Specifically, this task would involve letting a user run a model on an image and download sections of the image based on model output.

The aim is to support a wider range of models and flexible use of their outputs. One such example is a two stage CNN described here. Currently, caMicroscope supports single stage networks showing results directly, but no provision to use those results in any other model.

Current Status: Currently, caMicroscope supports uses of multiple types of models for markup, implemented with TensorFlow.js. Likewise, download of areas in an image given a bounding box is also supported.

Required Skills: JavaScript, TensorFlow.js (recommended)

Code Challenge: Using a machine learning toolkit of your choice, create a tool which identifies objects in the image, then returns positions in pixels corresponding to bounding boxes of a user-selected class of object in the image. For example, given an image with both cats and dogs, return bounding boxes for only cats.

Source Code: https://github.com/caMicroscope/caMicroscope

Slack Room: interest-extraction

