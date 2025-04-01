import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Mail, Github, Linkedin } from "lucide-react";

const Portfolio = () => {
  return (
    <div className="p-6 max-w-4xl mx-auto space-y-8">
      {/* About Section */}
      <Card>
        <CardContent className="p-6">
          <h1 className="text-3xl font-bold">Hello, I'm Yamini Velishala</h1>
          <p className="mt-2 text-gray-600">Highly motivated, ambitious, and organized individual seeking an entry-level position in the Software industry where I can utilize the extensive knowledge gained during my Bachelor's degree.</p>
        </CardContent>
      </Card>

      {/* Skills Section */}
      <Card>
        <CardContent className="p-6">
          <h2 className="text-2xl font-bold">Skills</h2>
          <ul className="mt-2 list-disc list-inside text-gray-600">
            <li>C</li>
            <li>Java</li>
            <li>Python</li>
            <li>JavaScript</li>
            <li>HTML & CSS</li>
            <li>MySQL</li>
          </ul>
        </CardContent>
      </Card>

      {/* Projects Section */}
      <Card>
        <CardContent className="p-6">
          <h2 className="text-2xl font-bold">Projects</h2>
          <div className="mt-2 space-y-4">
            <div>
              <h3 className="text-xl font-semibold">Detection of Malware in Android Applications using Machine Learning</h3>
              <p className="text-gray-600">Extracted relevant features from Android apps, prepared a dataset of good and bad apps, trained a machine learning model, and deployed it to detect malware threats in real-world applications.</p>
            </div>
          </div>
        </CardContent>
      </Card>

      {/* Contact Form */}
      <Card>
        <CardContent className="p-6">
          <h2 className="text-2xl font-bold">Contact Me</h2>
          <form className="mt-4 space-y-4">
            <input type="text" placeholder="Your Name" className="w-full p-2 border rounded-md" required />
            <input type="email" placeholder="Your Email" className="w-full p-2 border rounded-md" required />
            <textarea placeholder="Your Message" className="w-full p-2 border rounded-md" rows="4" required></textarea>
            <Button type="submit" className="w-full">Send Message</Button>
          </form>
        </CardContent>
      </Card>

      {/* Social Links */}
      <div className="flex justify-center space-x-4">
        <a href="mailto:velishalayamini17@gmail.com" className="text-gray-600 hover:text-black"><Mail /></a>
        <a href="https://github.com/" className="text-gray-600 hover:text-black"><Github /></a>
        <a href="https://www.linkedin.com/in/yamini-velishala-b03956254" className="text-gray-600 hover:text-black"><Linkedin /></a>
      </div>
    </div>
  );
};

export default Portfolio;
