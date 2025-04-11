import React from "react";
import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";
import { Input } from "@/components/ui/input";

export default function Home() {
  return (
    <div className="min-h-screen bg-white text-gray-900">
      <header className="p-6 shadow-md flex justify-between items-center">
        <h1 className="text-2xl font-bold">T.G Gîtes</h1>
        <nav className="space-x-4">
          <a href="#listings" className="hover:underline">Listings</a>
          <a href="#host" className="hover:underline">Become a Host</a>
          <a href="#contact" className="hover:underline">Contact</a>
        </nav>
      </header>

      <section className="p-8 text-center bg-gradient-to-r from-blue-100 to-blue-300">
        <h2 className="text-4xl font-bold mb-4">Holiday Houses in 4 Seasons, All Over the World</h2>
        <p className="text-lg max-w-2xl mx-auto">
          Discover unique stays across the globe. Clean, cozy, and listed directly by property owners.
        </p>
      </section>

      <section id="listings" className="p-8">
        <h3 className="text-2xl font-semibold mb-4">Featured Listings</h3>
        <div className="grid grid-cols-1 md:grid-cols-3 gap-6">
          <Card>
            <CardContent className="p-4">
              <img src="/placeholder-house.jpg" alt="House" className="rounded-xl mb-2" />
              <h4 className="text-lg font-semibold">Cozy Cabin in the Alps</h4>
              <p>Winter wonderland escape, sleeps 4.</p>
            </CardContent>
          </Card>
          <Card>
            <CardContent className="p-4">
              <img src="/placeholder-house2.jpg" alt="House" className="rounded-xl mb-2" />
              <h4 className="text-lg font-semibold">Beach House in Bali</h4>
              <p>Sunny vibes and tropical comfort.</p>
            </CardContent>
          </Card>
          <Card>
            <CardContent className="p-4">
              <img src="/placeholder-house3.jpg" alt="House" className="rounded-xl mb-2" />
              <h4 className="text-lg font-semibold">Countryside Cottage in France</h4>
              <p>Peaceful and picturesque, great for families.</p>
            </CardContent>
          </Card>
        </div>
      </section>

      <section id="host" className="p-8 bg-gray-100">
        <h3 className="text-2xl font-semibold mb-4">Become a Host</h3>
        <p className="mb-4">List your holiday house for just 99 Euros per year.</p>
        <Button className="bg-blue-600 text-white hover:bg-blue-700">
          Pay with Stripe
        </Button>
      </section>

      <section id="contact" className="p-8">
        <h3 className="text-2xl font-semibold mb-4">Contact Us</h3>
        <ul className="space-y-2">
          <li>Email: <a href="mailto:contact@tggites.com" className="text-blue-600">contact@tggites.com</a></li>
          <li>WhatsApp: <a href="https://wa.me/123456789" className="text-blue-600">Chat with us</a></li>
          <li>Facebook: <a href="https://facebook.com/tggites" className="text-blue-600">Follow us</a></li>
          <li>X (Twitter): <a href="https://x.com/tggites" className="text-blue-600">@tggites</a></li>
        </ul>
      </section>

      <footer className="p-4 text-center text-gray-500">
        &copy; 2025 T.G Gîtes. All rights reserved.
      </footer>
    </div>
  );
}
