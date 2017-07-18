TIL 7/15/17 The routes of a React web-app are contained in the app.js file, under the Router and Switch component tags. The route is coded as follows: 

import React, { Component } from 'react';
class App extends Component {
  render() {
    return (
      <div className="App">
          <Router>
            <Switch>
import {BrowserRouter as Router, Route, Switch} from 'react-router-dom';
<Route exact path="/" component={Home}></Route>


This is different from Rails, in which routes are contained in the config>routes file, and are coded as follows:

Rails.application.routes.draw do
  get '/' => 'contacts#index'

