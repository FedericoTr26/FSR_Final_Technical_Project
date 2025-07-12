# Robust Control of a Quadrotor UAV: Hierarchical vs Passivity-Based Approach

This repository presents the implementation and comparison of two control architectures for a quadrotor UAV:

- **Hierarchical Control**: based on a two-loop structure with an outer LQR controller for position and an inner PD controller for attitude.
- **Passivity-Based Control**: For robust stability.

Both control strategies are tested in two scenarios:
- **Without external disturbances**
- **With external disturbances (external wrench)**


## 🛠️ Requirements

- MATLAB R2023a or newer  
- Simulink  
- Control System Toolbox  
- 3D Animation Toolbox (optional, for UAV visualization)

## 🚀 How to Run

1. Open MATLAB.
2. Navigate to the desired controller folder (`Hierarchical/` or `Passivity/`).
3. Run one of the simulation scripts:
   ### Hierarchical Control:
   ```matlab
   run('main.m')           % without disturbance  
   run('main_wrench.m')    % with external disturbance
   ```
    ### Passivity-Based Control:
   ```matlab
   run('MainPassivityNoDisturbance.m')     % without disturbance  
   run('MainPassivityDisturbance.m')       % with external disturbance  
   ```

## 📊 Simulation Outputs

Each simulation automatically generates the following:

- 🛸 **3D UAV animation** during the execution of the trajectory tracking.
- 📈 **Plots** showing:
  - Reference trajectory
  - Position tracking 
  - Orientation tracking (Euler angles)
  - Control errors and stability behavior
- 💾 **EPS files** containing all plots, will be saved in the corresponding subfolder for documentation and report inclusion.

