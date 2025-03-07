import React from "react";
import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";
import { FaGithub, FaLinkedin, FaEnvelope } from "react-icons/fa";

export default function Portfolio() {
  return (
    <div className="min-h-screen bg-gray-100 flex flex-col items-center p-6">
      <Card className="max-w-3xl w-full bg-white shadow-xl p-6 rounded-2xl text-center">
        <img
          src="https://via.placeholder.com/150"
          alt="Profile"
          className="w-32 h-32 rounded-full mx-auto mb-4"
        />
        <h1 className="text-3xl font-bold mb-2">Your Name</h1>
        <p className="text-gray-600">Web Developer | Designer | Freelancer</p>
        <p className="mt-4 text-gray-500">
          Passionate about building interactive applications and experiences
        </p>
        <div className="mt-6 flex justify-center space-x-4">
          <Button variant="outline">
            <FaGithub className="mr-2" /> GitHub
          </Button>
          <Button variant="outline">
            <FaLinkedin className="mr-2" /> LinkedIn
          </Button>
          <Button variant="outline">
            <FaEnvelope className="mr-2" /> Contact
          </Button>
        </div>
      </Card>
    </div>
  );
}
