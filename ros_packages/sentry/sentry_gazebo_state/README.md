# sentry_gazebo_state

This node is a stand-in for a robot localization system, to be used for 
learning and code-development purposes only.  It assumes a mobile-robot model
called "sentry" is known to gazebo.  It subscribes to the topic
gazebo/model_states.  It searches the list of model names to find a match to "sentry".

It extracts the corresponding Pose from the model states, and re-publishes this
pose to the topic "gazebo_sentry_pose."

A steering algorithm can consult this topic for use in feedback, relative to
some path of interest.

## Example usage

`rosrun sentry_gazebo_state sentry_gazebo_state`

    
