classdef GUI_Terminada < matlab.apps.AppBase

    % Properties that correspond to app components
    properties (Access = public)
        UIFigure                  matlab.ui.Figure
        TabGroup2                 matlab.ui.container.TabGroup
        vsTab_2                   matlab.ui.container.Tab
        Label_17                  matlab.ui.control.Label
        CreadoporJosManuelSnchezMuozLabel_2  matlab.ui.control.Label
        IRNTextAreaLabel          matlab.ui.control.Label
        IRN_a_vs_IRN              matlab.ui.control.TextArea
        TextArea_16Label          matlab.ui.control.Label
        tetha_a_vs_IRN            matlab.ui.control.TextArea
        TextArea_15Label          matlab.ui.control.Label
        alfa_a_vs_IRN             matlab.ui.control.TextArea
        INTextAreaLabel           matlab.ui.control.Label
        IN_a_vs_IN                matlab.ui.control.TextArea
        TextArea_14Label          matlab.ui.control.Label
        tetha_a_vs_IN             matlab.ui.control.TextArea
        TextArea_13Label          matlab.ui.control.Label
        alfa_a_vs_IN              matlab.ui.control.TextArea
        Label_11                  matlab.ui.control.Label
        alfa_a_vs_g               matlab.ui.control.TextArea
        gama_a_vs_g               matlab.ui.control.TextArea
        Label_9                   matlab.ui.control.Label
        tetha_a_vs_g              matlab.ui.control.TextArea
        modo_alfa_vs_theta        matlab.ui.control.ToggleSwitch
        ModovsLabel               matlab.ui.control.Label
        modo_a_vs_IN              matlab.ui.control.ToggleSwitch
        ModovsINLabel             matlab.ui.control.Label
        modo_a_vs_IRN             matlab.ui.control.ToggleSwitch
        ModovsIRNLabel            matlab.ui.control.Label
        alfa_vs_IRN               matlab.ui.control.UIAxes
        alfa_vs_IN                matlab.ui.control.UIAxes
        alfa_vs_gama              matlab.ui.control.UIAxes
        Custom_IN_IRNTab_2        matlab.ui.container.Tab
        CreadoporJosManuelSnchezMuozLabel_3  matlab.ui.control.Label
        LLabel_2                  matlab.ui.control.Label
        L_text                    matlab.ui.control.TextArea
        RLabel                    matlab.ui.control.Label
        R_text                    matlab.ui.control.TextArea
        fLabel_3                  matlab.ui.control.Label
        f_text                    matlab.ui.control.TextArea
        VmaxLabel_2               matlab.ui.control.Label
        Vmax_text                 matlab.ui.control.TextArea
        Vo_RMS_out                matlab.ui.control.TextArea
        VoRMSLabel_3              matlab.ui.control.Label
        Vo_AVG_out                matlab.ui.control.TextArea
        VoAVGLabel_2              matlab.ui.control.Label
        Io_RMS_out                matlab.ui.control.TextArea
        IoRMSLabel_3              matlab.ui.control.Label
        IRNLabel                  matlab.ui.control.Label
        IRN_out                   matlab.ui.control.TextArea
        INLabel                   matlab.ui.control.Label
        IN_out                    matlab.ui.control.TextArea
        Label_14                  matlab.ui.control.Label
        teta_out                  matlab.ui.control.TextArea
        Label_13                  matlab.ui.control.Label
        beta_out                  matlab.ui.control.TextArea
        Label_12                  matlab.ui.control.Label
        alfa_text                 matlab.ui.control.TextArea
        Io_AVG_out                matlab.ui.control.TextArea
        IoAVGLabel                matlab.ui.control.Label
        Label_3                   matlab.ui.control.Label
        alfa_out                  matlab.ui.control.TextArea
        gama_out                  matlab.ui.control.TextArea
        mHLabel                   matlab.ui.control.Label
        DispararButton_4          matlab.ui.control.Button
        OUTPUTSLabel              matlab.ui.control.Label
        INPUTSLabel               matlab.ui.control.Label
        Label_16                  matlab.ui.control.Label
        alfa_vs_IRN_VAK           matlab.ui.control.UIAxes
        alfa_vs_IN_y_VL           matlab.ui.control.UIAxes
        alfa_vs_gama_y_corriente  matlab.ui.control.UIAxes
    end

    
    methods (Access = public)
        
        function clear_alfa_vs_IRN(app)
            cla(app.alfa_vs_IRN);  
            hold(app.alfa_vs_IRN, 'on'); 
            xlabel(app.alfa_vs_IRN, 'α', 'FontSize', 16);
            ylabel(app.alfa_vs_IRN, 'IRN', 'FontSize', 16);
            title(app.alfa_vs_IRN, 'α vs IRN', 'FontSize', 16);
            grid(app.alfa_vs_IRN, 'on');
            xlim(app.alfa_vs_IRN, [0 180]);
            xticks(app.alfa_vs_IRN, linspace(0, 180, 9));
            yticks_y = linspace(0, 1, 6); 
            yticks(app.alfa_vs_IRN, yticks_y);
            hold(app.alfa_vs_IRN, 'off');
        end
        
        function clear_alfa_vs_IN(app)
            cla(app.alfa_vs_IN);  
            hold(app.alfa_vs_IN, 'on');  
            xlabel(app.alfa_vs_IN, 'α', 'FontSize', 16);
            ylabel(app.alfa_vs_IN, 'IN', 'FontSize', 16);
            title(app.alfa_vs_IN, 'α vs IN', 'FontSize', 16);
            grid(app.alfa_vs_IN, 'on');
            xlim(app.alfa_vs_IN, [0 180]);
            xticks(app.alfa_vs_IN, linspace(0, 180, 9));
            yticks_y = linspace(0, 1, 6); 
            yticks(app.alfa_vs_IN, yticks_y);
            hold(app.alfa_vs_IN, 'off');
        end
        
        function clear_alfa_vs_gama(app)
            cla(app.alfa_vs_gama); % Limpiar el eje antes de graficar
            xlabel(app.alfa_vs_gama, 'α', 'FontSize', 16);
            ylabel(app.alfa_vs_gama, 'γ', 'FontSize', 13);
            title(app.alfa_vs_gama, 'α vs γ', 'FontSize', 16);
            grid(app.alfa_vs_gama, 'on');
            xlim(app.alfa_vs_gama, [0 180]);
            ticks = round(linspace(0, 180, 9)); % Redondear los valores a enteros
            xticks(app.alfa_vs_gama, ticks);
            yticks_y = linspace(0, 1, 6); 
            yticks(app.alfa_vs_gama, yticks_y);
            grados_labels = linspace(0, 180, 9);
            xticklabels(app.alfa_vs_gama, arrayfun(@num2str, grados_labels, 'UniformOutput', false));
            hold(app.alfa_vs_gama, 'off');
        end
        
        function clear_custom_plot_VAK(app)
            T_VL = 2*pi;
            cla(app.alfa_vs_IRN_VAK);
            hold(app.alfa_vs_IRN_VAK, 'on');
            xlabel(app.alfa_vs_IRN_VAK, 'Ángulo (grados)');
            ylabel(app.alfa_vs_IRN_VAK, 'VAK');
            title(app.alfa_vs_IRN_VAK, 'Voltaje en AK', 'FontSize', 16);
            grid(app.alfa_vs_IRN_VAK, 'on');
            xlim(app.alfa_vs_IRN_VAK, [0 T_VL]); 
            xticks(app.alfa_vs_IRN_VAK, linspace(0, T_VL, 9)); % 9 divisiones en el periodo
            yticks_y = linspace(0, 1, 6); 
            yticks(app.alfa_vs_IRN_VAK, yticks_y);
            grados_labels = linspace(0, 360, 9); % Etiquetas de grados
            xticklabels(app.alfa_vs_IRN_VAK, arrayfun(@num2str, grados_labels, 'UniformOutput', false));
            yticks_y = linspace(0, 1, 6); 
            yticks(app.alfa_vs_IRN_VAK, yticks_y);
            hold(app.alfa_vs_IRN_VAK, 'off');
        end
        
        function clear_custom_plot_VL(app)
            T_VL = 2*pi;
            cla(app.alfa_vs_IN_y_VL);
            hold(app.alfa_vs_IN_y_VL, 'on');
            xlabel(app.alfa_vs_IN_y_VL, 'Ángulo (grados)');
            ylabel(app.alfa_vs_IN_y_VL, 'Vo');
            title(app.alfa_vs_IN_y_VL, 'Voltaje en la carga', 'FontSize', 16);
            grid(app.alfa_vs_IN_y_VL, 'on');
            xlim(app.alfa_vs_IN_y_VL, [0 T_VL]); 
            xticks(app.alfa_vs_IN_y_VL, linspace(0, T_VL, 9)); % 9 divisiones en el periodo
            grados_labels = linspace(0, 360, 9); % Etiquetas de grados
            xticklabels(app.alfa_vs_IN_y_VL, arrayfun(@num2str, grados_labels, 'UniformOutput', false));
            yticks_y = linspace(0, 1, 6); 
            yticks(app.alfa_vs_IN_y_VL, yticks_y);
            hold(app.alfa_vs_IN_y_VL, 'off');
        end
        
        function clear_custom_plot_IL(app)
            T = 360;
            cla(app.alfa_vs_gama_y_corriente);
            hold(app.alfa_vs_gama_y_corriente, 'on');
            title(app.alfa_vs_gama_y_corriente, 'Corriente en la carga', 'FontSize', 16);
            xlabel(app.alfa_vs_gama_y_corriente, 'Ángulo (grados)');
            ylabel(app.alfa_vs_gama_y_corriente, 'Corriente');
            xlim(app.alfa_vs_gama_y_corriente, [0 T]); 
            xticks(app.alfa_vs_gama_y_corriente, linspace(0, T, 9)); 
            grados_labels = linspace(0, 360, 9); 
            xticklabels(app.alfa_vs_gama_y_corriente, arrayfun(@num2str, grados_labels, 'UniformOutput', false));
            yticks_y = linspace(0, 1, 6); 
            yticks(app.alfa_vs_gama_y_corriente, yticks_y);
            grid(app.alfa_vs_gama_y_corriente, 'on'); 
            hold(app.alfa_vs_gama_y_corriente, 'off');
            
        end
        
        
    end
    
    

    % Callbacks that handle component events
    methods (Access = private)

        % Code that executes after component creation
        function startupFcn(app)
            screenSize = get(0, 'ScreenSize');
            anchoPantalla = screenSize(3);
            anchoApp = app.UIFigure.Position(3);
            x = (anchoPantalla/2) - (anchoApp/2);
            app.UIFigure.Position(1) = x ; 
            app.UIFigure.Position(2) = 30;
            clear_alfa_vs_gama(app);
            clear_alfa_vs_IN(app);
            clear_alfa_vs_IRN(app);
            clear_custom_plot_VAK(app);
            clear_custom_plot_VL(app);
            clear_custom_plot_IL(app);
        end

        % Button pushed function: DispararButton_4
        function Custom_IN_IRNTabButtonDown(app, event)
            if  isempty(app.alfa_text.Value{1}) || isempty(app.f_text.Value{1}) || ...
                isempty(app.L_text.Value{1}) || isempty(app.Vmax_text.Value{1}) || ...
                isempty(app.R_text.Value{1})
                uialert(app.UIFigure, 'Todas las entradas deben estar llenas antes de continuar.', 'Error', 'Icon', 'error');
                return;
            end
            
            if any(cellfun(@(x) any(isletter(x)), {app.alfa_text.Value{1}, app.f_text.Value{1}, ...
               app.L_text.Value{1}, app.Vmax_text.Value{1}, ...
               app.R_text.Value{1}}))
                uialert(app.UIFigure, 'Solo se permiten números en las entradas.', 'Error', 'Icon', 'error');
                return;
            end
            
            R = str2double(app.R_text.Value);
            
            if R == 0
                uialert(app.UIFigure, 'El software no soporta entradas puramente inductivas.', 'Error', 'Icon', 'error');
                return;
            end
            
            Vmax = str2double(app.Vmax_text.Value);
            L = str2double(app.L_text.Value)/1000;
            f = str2double(app.f_text.Value);
            alfa = str2double(app.alfa_text.Value);
            
            if alfa == 180
                uialert(app.UIFigure, 'Si alfa es 180 grados, el circuito no recibe energía.', 'Error', 'Icon', 'error');
                return;
            end
            
            T = 1/f;
            w = 2 * pi * f;  
            X_L = w * L;  
            Z = sqrt(R^2 + X_L^2); 
            theta = atan(X_L / R); 
            resolucion = 100000;  
            theta_grados = theta*180/pi;
            
            beta = obtener_beta(alfa, T);
            gama = beta - alfa;
            
            [t_it, i_t_RL] = plot_I_t(alfa, beta, R, L, w, T, 100000, theta);
            plot_VL(alfa, beta);
            plot_VAK(alfa, beta);
            
            IN = obtener_IN(t_it, i_t_RL, w);
            IRN = obtener_IRN(t_it, i_t_RL);
            
            app.alfa_out.Value = sprintf('%.2f°', alfa);
            app.beta_out.Value = sprintf('%.2f°', beta); 
            app.teta_out.Value = sprintf('%.2f°', theta_grados); 
            app.gama_out.Value = sprintf('%.2f°', gama); 
            app.IN_out.Value = num2str(IN);
            app.IRN_out.Value = num2str(IRN);
            app.Io_AVG_out.Value = num2str(1000*obtener_io_AVG(IN)) + " mA";
            app.Io_RMS_out.Value = num2str(1000*obtener_io_RMS(IRN))+ " mA";
            app.Vo_AVG_out.Value = num2str(obtener_Vo_AVG(alfa, beta)) + " V";
            app.Vo_RMS_out.Value = num2str(obtener_Vo_RMS(alfa, beta)) + " V";
            
            if L == 0 
                carga_puramente_resistiva()
                Io_R_plot();
                Vo_R_plot();
                VAK_R_plot();
                return;
            end
            
            function cero_marker(grafica, alfa, f_t, Y_pos, x_pos)
                % grafica: el objeto de la gráfica en la que se va a dibujar
                % simbolo: 'alfa' o 'beta' como texto
                % x_pos: 'right' o 'left' o 'center' como texto

                % Dibujar líneas verticales en la posición alfa
                %line(grafica, [alfa alfa], [0 max_v*0.1], 'Color', 'm', 'LineWidth', 1.5, 'LineStyle', '-')
                %line(grafica, [alfa alfa], [0 -(max_v*0.1)], 'Color', 'm', 'LineWidth', 1.5, 'LineStyle', '-')
                
                etiqueta = sprintf('%.0f°', alfa);
            
                % Colocar la etiqueta en la gráfica
                if strcmp(Y_pos, 'up')
                    text(grafica, alfa, 0, etiqueta,...
                    'VerticalAlignment', 'bottom', 'HorizontalAlignment', x_pos, ...
                    'FontSize', 12, 'Color', 'm', 'Interpreter', 'latex'); % Activar LaTeX
                elseif strcmp(Y_pos, 'down')
                    text(grafica, alfa, 0, etiqueta,...
                    'VerticalAlignment', 'top', 'HorizontalAlignment', x_pos, ...
                    'FontSize', 12, 'Color', 'm', 'Interpreter', 'latex'); % Activar LaTeX
                end
            end
            
            function carga_puramente_resistiva()
                alfa_R = alfa;
                alfa_rad = deg2rad(alfa);
                beta_R = 180;
                theta_R = 0;
                gama_R = beta_R - alfa;
                Vo_AVG_R = (Vmax/(2*pi))*(1+cos(alfa_rad));
                Vo_RMS_R = Vmax*sqrt((1/(4*pi))*(pi-alfa_rad + (sin(2*alfa_rad)/2)));
                Io_AVG_R = Vo_AVG_R/R;
                Io_RMS_R = Vo_RMS_R/R;
                IN_R = (1+cos(alfa_rad))/(2*pi);
                IRN_R = sqrt((1/(4*pi))* (pi-alfa_rad+(sin(2*alfa_rad)/2)));
                app.alfa_out.Value = sprintf('%.2f°', alfa_R);
                app.beta_out.Value = sprintf('%.2f°', beta_R); 
                app.teta_out.Value = sprintf('%.2f°', theta_R); 
                app.gama_out.Value = sprintf('%.2f°', gama_R); 
                app.IN_out.Value = num2str(IN_R);
                app.IRN_out.Value = num2str(IRN_R);
                app.Io_AVG_out.Value = num2str(Io_AVG_R) + " Amp";
                app.Io_RMS_out.Value = num2str(Io_RMS_R)+ " Amp";
                app.Vo_AVG_out.Value = num2str(Vo_AVG_R) + " V";
                app.Vo_RMS_out.Value = num2str(Vo_RMS_R) + " V"; 
            end
            
            function VAK_R_plot()
                 alfa_R = alfa *T/360;
                 t = linspace(0,alfa_R,200);
                 VAK_R = (Vmax*sin(w*t));
                 t_R = t*360/T;
                 
                 t_R_2 = linspace(T/2,T,200);
                 VAK_R_2 = Vmax*sin(w*t_R_2);
                 t_R_2 = t_R_2*360/T;
                 
                 cla(app.alfa_vs_IRN_VAK);
                 hold(app.alfa_vs_IRN_VAK, 'on');
                title(app.alfa_vs_IRN_VAK, 'Voltaje en AK', 'FontSize', 16);
                plot(app.alfa_vs_IRN_VAK, t_R, VAK_R, 'g', 'LineWidth', 1.5);
                line(app.alfa_vs_IRN_VAK, [alfa alfa], [0 VAK_R(:, end)], 'Color', 'g', 'LineWidth', 1.5, 'LineStyle', '-');
                plot(app.alfa_vs_IRN_VAK, [alfa 360/2], [0 0], 'g', 'LineWidth', 1.5);
                plot(app.alfa_vs_IRN_VAK, t_R_2, VAK_R_2, 'g', 'LineWidth', 1.5);
                xlabel(app.alfa_vs_IRN_VAK, 'Ángulo (grados)');
                ylabel(app.alfa_vs_IRN_VAK, 'VAK');
                xlim(app.alfa_vs_IRN_VAK, [0 360]); 
                ylim(app.alfa_vs_IRN_VAK, [min(VAK_R_2)+min(VAK_R_2)*0.15, max(VAK_R)+max(VAK_R)*0.3]); 
                xticks(app.alfa_vs_IRN_VAK, linspace(0, 360, 9)); 
                yticks_y = linspace(min(VAK_R_2)-0.1, max(VAK_R)+0.1, 6); 
                yticks(app.alfa_vs_IRN_VAK, yticks_y); 
                yticklabels(app.alfa_vs_IRN_VAK, compose('%.2f', yticks_y));
                grid(app.alfa_vs_IRN_VAK, 'on'); 
                cero_marker(app.alfa_vs_IRN_VAK, alfa, t_R, 'down', 'center');
                cero_marker(app.alfa_vs_IRN_VAK, 360/2, t_R, 'up', 'center');
                
                hold(app.alfa_vs_IRN_VAK, 'off');
                 
            end
            
            function Vo_R_plot()
                 VAK = 1.1; % caida de voltaje del SCR
                 alfa_R = alfa *T/360;
                 t = linspace(alfa_R,T/2,200);
                 VL = (Vmax*sin(w*t))-VAK;
                 t = t*360/T;
                 cla(app.alfa_vs_IN_y_VL);
                 hold(app.alfa_vs_IN_y_VL, 'on');
                title(app.alfa_vs_IN_y_VL, 'Voltaje en la carga', 'FontSize', 16);
                plot(app.alfa_vs_IN_y_VL, [0 alfa], [0 0], 'r', 'LineWidth', 1.5);
                line(app.alfa_vs_IN_y_VL, [alfa alfa], [0 VL(1)], 'Color', 'r', 'LineWidth', 1.5, 'LineStyle', '-');
                plot(app.alfa_vs_IN_y_VL, t, VL, 'r', 'LineWidth', 1.5);
                plot(app.alfa_vs_IN_y_VL, [360/2 360], [0 0], 'r', 'LineWidth', 1.5);
                xlabel(app.alfa_vs_IN_y_VL, 'Ángulo (grados)');
                ylabel(app.alfa_vs_IN_y_VL, 'VL');
                xlim(app.alfa_vs_IN_y_VL, [0 360]); 
                ylim(app.alfa_vs_IN_y_VL, [min(VL)-max(VL)*0.15, max(VL)+max(VL)*0.15]); 
                xticks(app.alfa_vs_IN_y_VL, linspace(0, 360, 9)); 
                yticks_y = linspace(min(VL)-0.1, max(VL)+0.1, 6); 
                yticks(app.alfa_vs_IN_y_VL, yticks_y); 
                yticklabels(app.alfa_vs_IN_y_VL, compose('%.2f', yticks_y));
                grid(app.alfa_vs_IN_y_VL, 'on'); 
                cero_marker(app.alfa_vs_IN_y_VL, alfa, VL, 'down', 'center');
                cero_marker(app.alfa_vs_IN_y_VL, 360/2, VL, 'down', 'center');
                hold(app.alfa_vs_IN_y_VL, 'off');
                 
            end
            
            function Io_R_plot()
                alfa_R = alfa *T/360;
                t = linspace(alfa_R,T/2,200);
                i = (Vmax/R)*sin(w*t);
                 t = t*360/T;
                 
                cla(app.alfa_vs_gama_y_corriente);
                hold(app.alfa_vs_gama_y_corriente, 'on');
                title(app.alfa_vs_gama_y_corriente, 'Corriente en la carga', 'FontSize', 16);
                plot(app.alfa_vs_gama_y_corriente, [0 alfa], [0 0], 'b', 'LineWidth', 1.5);
                line(app.alfa_vs_gama_y_corriente, [alfa alfa], [0 i(1)], 'Color', 'b', 'LineWidth', 1.5, 'LineStyle', '-');
                plot(app.alfa_vs_gama_y_corriente, t, i, 'b', 'LineWidth', 1.5);
                plot(app.alfa_vs_gama_y_corriente, [360/2 360], [0 0], 'b', 'LineWidth', 1.5);
                xlabel(app.alfa_vs_gama_y_corriente, 'Ángulo (grados)');
                ylabel(app.alfa_vs_gama_y_corriente, 'Corriente');
                xlim(app.alfa_vs_gama_y_corriente, [0 360]); 
                ylim(app.alfa_vs_gama_y_corriente, [min(i)-max(i)*0.15, max(i)+max(i)*0.15]); 
                xticks(app.alfa_vs_gama_y_corriente, linspace(0, 360, 9)); 
                grados_labels = linspace(0, 360, 9); 
                xticklabels(app.alfa_vs_gama_y_corriente, arrayfun(@num2str, grados_labels, 'UniformOutput', false));
                yticks_y = linspace(min(i)-0.1, max(i)+0.1, 6); 
                yticks(app.alfa_vs_gama_y_corriente, yticks_y); 
                yticklabels(app.alfa_vs_gama_y_corriente, compose('%.2f', yticks_y));
                grid(app.alfa_vs_gama_y_corriente, 'on'); 
                cero_marker(app.alfa_vs_gama_y_corriente, alfa, i, 'down', 'center');
                cero_marker(app.alfa_vs_gama_y_corriente, 360/2, i, 'down', 'center');
                hold(app.alfa_vs_gama_y_corriente, 'off');
            end
            
            
            
            function Vo_RMS = obtener_Vo_RMS(alfa, beta)
                alfa_rad = deg2rad(alfa);
                beta_rad = deg2rad(beta);
                Vo_RMS = Vmax*sqrt((1/(4*pi))*(beta_rad - alfa_rad + (sin(2*alfa_rad)/2) - (sin(2*beta_rad)/2)));
            end
            
            function Vo_AVG = obtener_Vo_AVG(alfa_Vo, beta_Vo)
                Vo_AVG = (Vmax/(2*pi))*(cos(deg2rad(alfa_Vo))-cos(deg2rad(beta_Vo)));
            end
            
            function io_RMS = obtener_io_RMS(IRN)
                io_RMS = (Vmax/Z)*IRN;
            end
            
            function io_AVG = obtener_io_AVG(IN)
                io_AVG = (Vmax/Z)*IN;
            end
            
            function plot_VAK(alfa, beta)
                T_VL = 360;
                VAK = 1.1; % caida de voltaje del SCR
                 
                alfa_VL = alfa * T / 360; 
                beta_VL = beta * T / 360;
                t_VL = linspace(0, alfa_VL, alfa);
                V_t = (Vmax - VAK) * sin(w * t_VL); % calcular el voltaje
                t_VL = t_VL*360/T;
                
                t_VL_2 = linspace(beta_VL, T, (360-beta));
                V_t_2 = (Vmax - VAK) * sin(w * t_VL_2); % calcular el voltaje
                t_VL_2 = t_VL_2*360/T;
                
                cla(app.alfa_vs_IRN_VAK);
                hold(app.alfa_vs_IRN_VAK, 'on');
                plot(app.alfa_vs_IRN_VAK, t_VL , V_t, 'g', 'LineWidth', 1.5); % Multiplicar por w para ajustar
                line(app.alfa_vs_IRN_VAK, [alfa alfa], [0 V_t(:, end)], 'Color', 'g', 'LineWidth', 1.5, 'LineStyle', '-');
                plot(app.alfa_vs_IRN_VAK, [alfa beta], [0 0], 'g', 'LineWidth', 1.5);
                line(app.alfa_vs_IRN_VAK, [beta beta], [0 V_t_2(1)], 'Color', 'g', 'LineWidth', 1.5, 'LineStyle', '-');
                
                plot(app.alfa_vs_IRN_VAK, t_VL_2, V_t_2, 'g', 'LineWidth', 1.5);
                xlabel(app.alfa_vs_IRN_VAK, 'Ángulo (grados)');
                ylabel(app.alfa_vs_IRN_VAK, 'VAK');
                title(app.alfa_vs_IRN_VAK, 'Voltaje en AK','FontSize', 16);
                grid(app.alfa_vs_IRN_VAK, 'on');
                xlim(app.alfa_vs_IRN_VAK, [0 T_VL]); 
                ylim(app.alfa_vs_IRN_VAK, [min(V_t_2)+min(V_t_2)*0.15, max(V_t)+max(V_t)*0.3]);
                xticks(app.alfa_vs_IRN_VAK, linspace(0, T_VL, 9)); % 9 divisiones en el periodo
                yticks_y = linspace(min(V_t_2)-0.1, max(V_t)+0.1, 6); 
                yticks(app.alfa_vs_IRN_VAK, yticks_y);
                yticklabels(app.alfa_vs_IRN_VAK, compose('%.2f', yticks_y));
                grados_labels = linspace(0, 360, 9); % Etiquetas de grados
                xticklabels(app.alfa_vs_IRN_VAK, arrayfun(@num2str, grados_labels, 'UniformOutput', false));
                
                cero_marker(app.alfa_vs_IRN_VAK, alfa, V_t_2, 'down', 'center');
                cero_marker(app.alfa_vs_IRN_VAK, beta, V_t_2, 'up', 'center');
                
                hold(app.alfa_vs_IRN_VAK, 'off');
                
            end
            
            function plot_VL(alfa, beta)
                T_VL = 360;
                VAK = 1.1; % caida de voltaje del SCR
                 
                alfa_VL = alfa * T / 360; 
                beta_VL = beta * T / 360;
                t_VL = linspace(alfa_VL, beta_VL, (beta-alfa));
                V_t = (Vmax - VAK) * sin(w * t_VL); % calcular el voltaje
                t_VL = t_VL*360/T;
                
                % Graficar
                cla(app.alfa_vs_IN_y_VL);
                hold(app.alfa_vs_IN_y_VL, 'on');
                plot(app.alfa_vs_IN_y_VL, [0 alfa], [0 0], 'r', 'LineWidth', 1.5);
                line(app.alfa_vs_IN_y_VL, [alfa alfa], [0 V_t(1)], 'Color', 'r', 'LineWidth', 1.5, 'LineStyle', '-');
                plot(app.alfa_vs_IN_y_VL, t_VL, V_t, 'r', 'LineWidth', 1.5); % Multiplicar por w para ajustar
                line(app.alfa_vs_IN_y_VL, [beta beta], [0 V_t(:, end)], 'Color', 'r', 'LineWidth', 1.5, 'LineStyle', '-');
                plot(app.alfa_vs_IN_y_VL, [beta T_VL], [0 0], 'r', 'LineWidth', 1.5);
                xlabel(app.alfa_vs_IN_y_VL, 'Ángulo (grados)');
                ylabel(app.alfa_vs_IN_y_VL, 'VL');
                title(app.alfa_vs_IN_y_VL, 'Voltaje en la carga','FontSize', 16);
                grid(app.alfa_vs_IN_y_VL, 'on');
                xlim(app.alfa_vs_IN_y_VL, [0 T_VL]); 
                ylim(app.alfa_vs_IN_y_VL, [min(V_t)-max(V_t)*0.15, max(V_t)+max(V_t)*0.15]); 
                xticks(app.alfa_vs_IN_y_VL, linspace(0, T_VL, 9)); % 9 divisiones en el periodo
                yticks_y = linspace(min(V_t), max(V_t), 6); 
                yticks(app.alfa_vs_IN_y_VL, yticks_y); 
                yticklabels(app.alfa_vs_IN_y_VL, compose('%.2f', yticks_y));
                grados_labels = linspace(0, 360, 9); % Etiquetas de grados
                xticklabels(app.alfa_vs_IN_y_VL, arrayfun(@num2str, grados_labels, 'UniformOutput', false));
                cero_marker(app.alfa_vs_IN_y_VL, alfa, V_t, 'down', 'center');
                cero_marker(app.alfa_vs_IN_y_VL, beta, V_t, 'up', 'center');
                
                hold(app.alfa_vs_IN_y_VL, 'off');
                
                
            end
            
            function IN = obtener_IN(t, i_t, w) 
                wt = w * t;  
                IN = (1/(2*pi)) * trapz(wt, i_t);  
            end
            
            function IRN = obtener_IRN(t, i_t) 
                wt = w * t;  
                IRN = sqrt((1/(2*pi)) * trapz(wt, i_t.^2));  
            end
            
            function [t, i_t] = plot_I_t(alfa, beta, R, L, w, T, resolucion, theta)  
                alfa_rad = alfa * (2 * pi) / 360;
                t_disparo = alfa * T / 360; 
                beta_rad = beta * T / 360;
                t = linspace(t_disparo, beta_rad, resolucion);
                
                % Genera la corriente i(t) en función de alfa y beta
                i_t = sin(w * t - theta) - sin(alfa_rad - theta) * exp((R / L) * ((alfa_rad / w) - t));
                t = t*360/T;
                
                i_t_plot = (Vmax/Z)*i_t;
                cla(app.alfa_vs_gama_y_corriente);
                hold(app.alfa_vs_gama_y_corriente, 'on');
                title(app.alfa_vs_gama_y_corriente, 'Corriente en la carga', 'FontSize', 16);
                plot(app.alfa_vs_gama_y_corriente, [0 alfa], [0 0], 'b', 'LineWidth', 1.5);
                plot(app.alfa_vs_gama_y_corriente, t, i_t_plot, 'b', 'LineWidth', 1.5);
                plot(app.alfa_vs_gama_y_corriente, [beta 360], [0 0], 'b', 'LineWidth', 1.5);
                xlabel(app.alfa_vs_gama_y_corriente, 'Ángulo (grados)');
                ylabel(app.alfa_vs_gama_y_corriente, 'Corriente');
                
                
                xlim(app.alfa_vs_gama_y_corriente, [0 360]); 
                ylim(app.alfa_vs_gama_y_corriente, [min(i_t_plot)-max(i_t_plot)*0.15, max(i_t_plot)+max(i_t_plot)*0.15]); %modificacion
            
      
                xticks(app.alfa_vs_gama_y_corriente, linspace(0, 360, 9)); 
                grados_labels = linspace(0, 360, 9); 
                xticklabels(app.alfa_vs_gama_y_corriente, arrayfun(@num2str, grados_labels, 'UniformOutput', false));
                yticks_y = linspace(min(i_t_plot), max(i_t_plot), 6); 
                yticks(app.alfa_vs_gama_y_corriente, yticks_y); 
                yticklabels(app.alfa_vs_gama_y_corriente, compose('%.2f', yticks_y));
                grid(app.alfa_vs_gama_y_corriente, 'on'); 
                
                cero_marker(app.alfa_vs_gama_y_corriente, alfa, i_t, 'down', 'center');
                cero_marker(app.alfa_vs_gama_y_corriente, beta, i_t, 'down', 'center');
                
                hold(app.alfa_vs_gama_y_corriente, 'off');
                t = linspace(t_disparo, beta_rad, resolucion);
            end
            
            function time = obtener_beta(angulo_de_disparo, periodo)
                alfa_2 = angulo_de_disparo * (2 * pi) / 360;
                t_disparo = angulo_de_disparo * (1/60) / 360;  
                t_beta = linspace(t_disparo, periodo, resolucion);
                i_t = (sin(w * t_beta - theta) - sin(alfa_2 - theta) * exp((R / L) * ((alfa_2 / w) - (t_beta))));
                
                tiempo_cruce = NaN;
                tiempo_anterior = NaN;
                primer_valor_encontrado = false;
            
                for i = 1:length(i_t)
                    
                    if ~primer_valor_encontrado && i_t(i) > 0
                        primer_valor_encontrado = true; 
                        continue; 
                    end
                    
                    if primer_valor_encontrado
                    
                        if i_t(i) < 0
                            
                            tiempo_cruce = t_beta(i);
                            if i > 1
                                tiempo_anterior = t_beta(i-1);
                            end
                            break; 
                        end
                    end
                end
                
                if ~isnan(tiempo_cruce) && ~isnan(tiempo_anterior)
                    time = (tiempo_cruce + tiempo_anterior) / 2;
                    time = time*360/periodo;
                else
                    time = NaN; 
                end
            end


           
        end

        % Value changed function: modo_alfa_vs_theta
        function modo_alfa_vs_thetaValueChanged(app, event)
                if  isempty(app.alfa_a_vs_g.Value{1}) || isempty(app.tetha_a_vs_g.Value{1})
                    uialert(app.UIFigure, 'Todas las entradas deben estar llenas antes de continuar.', 'Error', 'Icon', 'error');
                    return;
                end  
                
                if any(cellfun(@(x) any(isletter(x)), {app.alfa_a_vs_g.Value{1}, app.tetha_a_vs_g.Value{1}}))
                    uialert(app.UIFigure, 'Solo se permiten números en las entradas.', 'Error', 'Icon', 'error');
                    return;
                end
                
                alfa = str2double(app.alfa_a_vs_g.Value);
                theta = str2double(app.tetha_a_vs_g.Value);
                
                if alfa < 0 || alfa > 180
                    uialert(app.UIFigure, 'Alfa debe estar entre 0 y 180 grados.', 'Error', 'Icon', 'error');
                    return;
                end
                
                if theta < 0 || theta > 90
                    uialert(app.UIFigure, 'Theta debe estar entre 0 y 90 grados.', 'Error', 'Icon', 'error');
                    return;
                end
                
                if alfa == 180
                    app.gama_a_vs_g.Value = '0';
                    clear_alfa_vs_gama(app);
                    return;
                end
                
                app.gama_a_vs_g.Value = num2str(obtener_gama(alfa, theta, 100000));
                
                alfa_plot = 0:180;
                graficar_alfa_y_gama(alfa_plot, theta);

            function graficar_alfa_y_gama(alfa_plot, theta)
                
                gama_plot = zeros(1, length(alfa_plot));
                for idx = 1:length(alfa_plot)
                    gama_plot(idx) = obtener_gama(idx, theta, 10000);
                end
                
          
                cla(app.alfa_vs_gama); % Limpiar el eje antes de graficar
                plot(app.alfa_vs_gama, alfa_plot, gama_plot, 'b', 'LineWidth', 1.5);
                xlabel(app.alfa_vs_gama, 'α', 'FontSize', 16);
                ylabel(app.alfa_vs_gama, 'γ', 'FontSize', 13);
                title(app.alfa_vs_gama, 'α vs γ', 'FontSize', 16);
                grid(app.alfa_vs_gama, 'on');
                xlim(app.alfa_vs_gama, [0 180]);
                ticks = round(linspace(0, 180, 9)); % Redondear los valores a enteros
                xticks(app.alfa_vs_gama, ticks);
                %ticks = round(linspace(0, 360, 6));
                ylim(app.alfa_vs_gama, [min(gama_plot)-max(gama_plot)*0.15, max(gama_plot)+max(gama_plot)*0.15]); 
                yticks_y = linspace(min(gama_plot), max(gama_plot), 6); 
                yticks(app.alfa_vs_gama, yticks_y);
                %yticklabels(app.alfa_vs_gama, compose('%.2f', yticks));
                grados_labels = linspace(0, 180, 9);
                xticklabels(app.alfa_vs_gama, arrayfun(@num2str, grados_labels, 'UniformOutput', false));
                yticklabels(app.alfa_vs_gama, compose('%.2f', yticks_y));
                
            end
            
            function gama = obtener_gama(alfa, theta, resolucion)
                f = 60;   
                T = 1/f;       % Periodo
                L = 1;          % Inductancia
                w = 2 * pi * f; % Frecuencia angular
                X_L = w * L;  
                R = X_L / tan(deg2rad(theta));   
                
                alfa_2 = deg2rad(alfa);
                t_disparo = alfa * (1/60) / 360;  
                t = linspace(t_disparo, T, resolucion);
                i_t = (sin(w * t - deg2rad(theta)) - sin(alfa_2 - deg2rad(theta)) * exp((R / L) * ((alfa_2 / w) - (t))));
                
                tiempo_cruce = NaN;
                tiempo_anterior = NaN;
                primer_valor_encontrado = false;
            
                for i = 1:length(i_t)
                    
                    if ~primer_valor_encontrado && i_t(i) > 0
                        primer_valor_encontrado = true; 
                        continue; 
                    end
                    
                    if primer_valor_encontrado
                    
                        if i_t(i) < 0
                            
                            tiempo_cruce = t(i);
                            if i > 1
                                tiempo_anterior = t(i-1);
                            end
                            break; 
                        end
                    end
                end
                
                if ~isnan(tiempo_cruce) && ~isnan(tiempo_anterior)
                    time = (tiempo_cruce + tiempo_anterior) / 2;
                    gama = (time*360/T) - alfa;
                else
                    gama = NaN; 
                end
            end
        end

        % Value changed function: modo_a_vs_IN
        function modo_a_vs_INValueChanged(app, event)
            if  isempty(app.alfa_a_vs_IN.Value{1}) || isempty(app.tetha_a_vs_IN.Value{1})
                uialert(app.UIFigure, 'Todas las entradas deben estar llenas antes de continuar.', 'Error', 'Icon', 'error');
                return;
            end
            
            if any(cellfun(@(x) any(isletter(x)), {app.alfa_a_vs_IN.Value{1}, app.tetha_a_vs_IN.Value{1}}))
                uialert(app.UIFigure, 'Solo se permiten números en las entradas.', 'Error', 'Icon', 'error');
                return;
            end
            
            alfa = str2double(app.alfa_a_vs_IN.Value);
            theta = str2double(app.tetha_a_vs_IN.Value);
            app.IN_a_vs_IN.Value = num2str(calcular_IN(alfa, theta, 100000));
            
            if theta == 0
                uialert(app.UIFigure, 'Theta no puede ser 0 grados.', 'Error', 'Icon', 'error');
                return;
            end
            
            if alfa < 0 || alfa > 180
                uialert(app.UIFigure, 'Alfa debe estar entre 0 y 180 grados.', 'Error', 'Icon', 'error');
                return;
            end
            
            if theta < 0 || theta > 90
                uialert(app.UIFigure, 'Theta  debe estar entre 0 y 90 grados.', 'Error', 'Icon', 'error');
                return;
            end
            
            if alfa == 180
                app.IN_a_vs_IN.Value = '0';
                clear_alfa_vs_IN(app)
                return;
            end
        
            alfa_plot = 0:180;
            graficar_alfa_y_IN(alfa_plot, theta);
        
            function graficar_alfa_y_IN(alfa, theta)
                IN = zeros(1, length(alfa));
                for i = alfa
                    IN(i + 1) = calcular_IN(i, theta, 10000);
                end
        
                cla(app.alfa_vs_IN);  % Asegurar limpieza del `axes` específico
                hold(app.alfa_vs_IN, 'on');  % Evitar la creación de nueva figura
                plot(app.alfa_vs_IN, alfa, IN, 'r', 'LineWidth', 1.5);
                xlabel(app.alfa_vs_IN, 'α', 'FontSize', 16);
                ylabel(app.alfa_vs_IN, 'IN', 'FontSize', 16);
                title(app.alfa_vs_IN, 'α vs IN', 'FontSize', 16);
                grid(app.alfa_vs_IN, 'on');
                xlim(app.alfa_vs_IN, [0 180]);
                xticks(app.alfa_vs_IN, linspace(0, 180, 9));
                ylim(app.alfa_vs_IN, [min(IN)-max(IN)*0.15, max(IN)+max(IN)*0.15]); 
                yticks_y = linspace(min(IN), max(IN), 6); 
                yticks(app.alfa_vs_IN, yticks_y);
                yticklabels(app.alfa_vs_IN, compose('%.2f', yticks_y));
                hold(app.alfa_vs_IN, 'off');
            end
        
            % Mantener el resto de funciones sin cambios
            function IN = calcular_IN(alfa, theta, resolucion)
                beta = obtener_beta(alfa, theta);
                [t, i_t] = calcular_I_t(alfa, beta, deg2rad(theta), resolucion);
                wt = 2 * pi * 60 * t;  
                IN = (1 / (2 * pi)) * trapz(wt, i_t);
            end
        
            function [t, i_t] = calcular_I_t(alfa, beta, theta, resolucion)
                f = 60;   
                T = 1 / f;     
                L = 1;
                w = 2 * pi * f;
                X_L = w * L;
                R = X_L / tan(theta);
        
                alfa_2 = alfa * (2 * pi) / 360;
                t_disparo = alfa * T / 360;
                beta = beta * T / 360;
                t = linspace(t_disparo, beta, resolucion);
                i_t = sin(w * t - theta) - sin(alfa_2 - theta) * exp((R / L) * ((alfa_2 / w) - t));
            end
        
            function beta = obtener_beta(alfa, theta)   
                f = 60;   
                T = 1 / f;
                L = 1;
                w = 2 * pi * f;
                X_L = w * L;
                R = X_L / tan(deg2rad(theta));
                resolucion = 100000;
        
                alfa_2 = deg2rad(alfa);
                t_disparo = alfa * (1 / 60) / 360;
                t = linspace(t_disparo, T, resolucion);
                i_t = (sin(w * t - deg2rad(theta)) - sin(alfa_2 - deg2rad(theta)) * exp((R / L) * ((alfa_2 / w) - t)));
        
                tiempo_cruce = NaN;
                tiempo_anterior = NaN;
                primer_valor_encontrado = false;
        
                for i = 1:length(i_t)
                    if ~primer_valor_encontrado && i_t(i) > 0
                        primer_valor_encontrado = true; 
                        continue; 
                    end
        
                    if primer_valor_encontrado
                        if i_t(i) < 0
                            tiempo_cruce = t(i);
                            if i > 1
                                tiempo_anterior = t(i - 1);
                            end
                            break; 
                        end
                    end
                end
        
                if ~isnan(tiempo_cruce) && ~isnan(tiempo_anterior)
                    time = (tiempo_cruce + tiempo_anterior) / 2;
                    beta = time * 360 / T;
                else
                    beta = NaN;
                end
            end
        end

        % Value changed function: modo_a_vs_IRN
        function modo_a_vs_IRNValueChanged(app, event)
            if  isempty(app.alfa_a_vs_IRN.Value{1}) || isempty(app.tetha_a_vs_IRN.Value{1})
                uialert(app.UIFigure, 'Todas las entradas deben estar llenas antes de continuar.', 'Error', 'Icon', 'error');
                return;
            end
            
             if any(cellfun(@(x) any(isletter(x)), {app.alfa_a_vs_IRN.Value{1}, app.tetha_a_vs_IRN.Value{1}}))
                uialert(app.UIFigure, 'Solo se permiten números en las entradas.', 'Error', 'Icon', 'error');
                return;
             end
            
            alfa = str2double(app.alfa_a_vs_IRN.Value);
            theta = str2double(app.tetha_a_vs_IRN.Value);
            app.IRN_a_vs_IRN.Value  = num2str(calcular_IRN(alfa, theta, 100000)); 
            
            if theta == 0
                uialert(app.UIFigure, 'Theta no puede ser 0 grados.', 'Error', 'Icon', 'error');
                return;
            end
            
            if alfa < 0 || alfa > 180
                uialert(app.UIFigure, 'Alfa debe estar entre 0 y 180 grados.', 'Error', 'Icon', 'error');
                return;
            end
            
            if theta < 0 || theta > 90
                uialert(app.UIFigure, 'Theta  debe estar entre 0 y 90 grados.', 'Error', 'Icon', 'error');
                return;
            end
            
            if alfa == 180 
                app.IRN_a_vs_IRN.Value = '0';
                clear_alfa_vs_IRN(app);
                return;
            end
            
            alfa_plot = 0:180;
            graficar_alfa_y_IRN(alfa_plot, theta);
        
            function graficar_alfa_y_IRN(alfa, theta)
                IRN = zeros(1, length(alfa));
                for i = alfa
                    IRN(i + 1) = calcular_IRN(i, theta, 10000);
                end
        
                cla(app.alfa_vs_IRN);  % Asegurar limpieza del `axes` específico
                hold(app.alfa_vs_IRN, 'on');  % Evitar la creación de nueva figura
                plot(app.alfa_vs_IRN, alfa, IRN, 'g', 'LineWidth', 1.5);
                xlabel(app.alfa_vs_IRN, 'α', 'FontSize', 16);
                ylabel(app.alfa_vs_IRN, 'IRN', 'FontSize', 16);
                title(app.alfa_vs_IRN, 'α vs IRN', 'FontSize', 16);
                grid(app.alfa_vs_IRN, 'on');
                xlim(app.alfa_vs_IRN, [0 180]);
                ylim(app.alfa_vs_IRN, [min(IRN)-max(IRN)*0.15, max(IRN)+max(IRN)*0.15]); 
                xticks(app.alfa_vs_IRN, linspace(0, 180, 9));
                yticks_y = linspace(min(IRN), max(IRN), 6); 
                yticks(app.alfa_vs_IRN, yticks_y); 
                yticklabels(app.alfa_vs_IRN, compose('%.2f', yticks_y));
                hold(app.alfa_vs_IRN, 'off');
            end
           
            function IRN = calcular_IRN(alfa, theta, resolucion)
                beta = obtener_beta(alfa, theta);
                [t, i_t] = calcular_I_t(alfa, beta, deg2rad(theta), resolucion);
                
                wt = 2 * pi*60 * t;  
                IRN = sqrt((1/(2*pi)) * trapz(wt, i_t.^2));  
                
            end
            
            function [t, i_t] = calcular_I_t(alfa, beta, theta, resolucion)   
                f = 60;   
                T = 1/f;       % Periodo
                L = 1;          % Inductancia
                w = 2 * pi * f; % Frecuencia angular
                X_L = w * L;  
                R = X_L / tan(theta); 
                
                alfa_2 = alfa * (2 * pi) / 360;
                t_disparo = alfa * T/360; 
                beta = beta * T/360;
                t = linspace(t_disparo, beta, resolucion);
                i_t = sin(w * t - theta) - sin(alfa_2 - theta) * exp((R / L) * ((alfa_2 / w) - (t)));
                
            end
            
            function beta = obtener_beta(alfa, theta)
                  
                f = 60;   
                T = 1/f;      
                L = 1;          
                w = 2 * pi * f; 
                X_L = w * L;  
                R = X_L / tan(deg2rad(theta)); 
                resolucion = 100000;  
                
                alfa_2 = deg2rad(alfa);
                t_disparo = alfa * (1/60) / 360;  
                t = linspace(t_disparo, T, resolucion);
                i_t = (sin(w * t - deg2rad(theta)) - sin(alfa_2 - deg2rad(theta)) * exp((R / L) * ((alfa_2 / w) - (t))));
                
                tiempo_cruce = NaN;
                tiempo_anterior = NaN;
                primer_valor_encontrado = false;
            
                for i = 1:length(i_t)
                    
                    if ~primer_valor_encontrado && i_t(i) > 0
                        primer_valor_encontrado = true; 
                        continue; 
                    end
                    
                    if primer_valor_encontrado
                    
                        if i_t(i) < 0
                            
                            tiempo_cruce = t(i);
                            if i > 1
                                tiempo_anterior = t(i-1);
                            end
                            break; 
                        end
                    end
                end
                
                if ~isnan(tiempo_cruce) && ~isnan(tiempo_anterior)
                    time = (tiempo_cruce + tiempo_anterior) / 2;
                    beta = time*360/T;
                else
                    beta = NaN; 
                end
            end
        end

        % Callback function
        function UIFigureSizeChanged(app, event)

            screenSize = get(0, 'ScreenSize');
    
            % Ajustar el tamaño de la figura a la pantalla completa
            app.UIFigure.Position = [0, 0, screenSize(3), screenSize(4)];
        end

        % Callback function
        function UIFigureSizeChanged2(app, event)
          
            
        end

        % Callback function
        function Custom_IN_IRNTab_2ButtonDown(app, event)
          
        end

        % Callback function
        function vsTab_2ButtonDown(app, event)
            if ~isempty(app.alfa_a_vs_g.Value{1}) && ~isempty(app.tetha_a_vs_g.Value{1})
                modo_alfa_vs_thetaValueChanged(app, event);
            else 
                clear_alfa_vs_gama(app);
            end
        
            if ~isempty(app.alfa_a_vs_IN.Value{1}) && ~isempty(app.tetha_a_vs_IN.Value{1})
                modo_a_vs_INValueChanged(app, event);
            else
                clear_alfa_vs_IN(app);
            end
        
            if ~isempty(app.alfa_a_vs_IRN.Value{1}) && ~isempty(app.tetha_a_vs_IRN.Value{1})
                modo_a_vs_IRNValueChanged(app, event);
            else
                clear_alfa_vs_IRN(app);
            end

        end

        % Callback function
        function Custom_IN_IRNTab_2ButtonDown2(app, event)

            if ~isempty(app.alfa_text.Value{1}) && ~isempty(app.f_text.Value{1}) && ...
               ~isempty(app.L_text.Value{1}) && ~isempty(app.Vmax_text.Value{1}) && ...
               ~isempty(app.R_text.Value{1})
               Custom_IN_IRNTabButtonDown(app, event);
            else
                clear_custom_plot_VAK(app);
                clear_custom_plot_VL(app);
                clear_custom_plot_IL(app);
            end 
        end
    end

    % Component initialization
    methods (Access = private)

        % Create UIFigure and components
        function createComponents(app)

            % Create UIFigure and hide until all components are created
            app.UIFigure = uifigure('Visible', 'off');
            app.UIFigure.Position = [100 100 840 660];
            app.UIFigure.Name = 'MATLAB App';

            % Create TabGroup2
            app.TabGroup2 = uitabgroup(app.UIFigure);
            app.TabGroup2.Position = [1 -14 840 675];

            % Create vsTab_2
            app.vsTab_2 = uitab(app.TabGroup2);
            app.vsTab_2.Title = 'α vs θ';

            % Create alfa_vs_gama
            app.alfa_vs_gama = uiaxes(app.vsTab_2);
            title(app.alfa_vs_gama, 'Title')
            xlabel(app.alfa_vs_gama, 'X')
            ylabel(app.alfa_vs_gama, 'Y')
            zlabel(app.alfa_vs_gama, 'Z')
            app.alfa_vs_gama.Position = [26 435 518 202];

            % Create alfa_vs_IN
            app.alfa_vs_IN = uiaxes(app.vsTab_2);
            title(app.alfa_vs_IN, 'Title')
            xlabel(app.alfa_vs_IN, 'X')
            ylabel(app.alfa_vs_IN, 'Y')
            zlabel(app.alfa_vs_IN, 'Z')
            app.alfa_vs_IN.Position = [26 233 518 202];

            % Create alfa_vs_IRN
            app.alfa_vs_IRN = uiaxes(app.vsTab_2);
            title(app.alfa_vs_IRN, 'Title')
            xlabel(app.alfa_vs_IRN, 'X')
            ylabel(app.alfa_vs_IRN, 'Y')
            zlabel(app.alfa_vs_IRN, 'Z')
            app.alfa_vs_IRN.Position = [26 25 518 202];

            % Create ModovsIRNLabel
            app.ModovsIRNLabel = uilabel(app.vsTab_2);
            app.ModovsIRNLabel.HorizontalAlignment = 'center';
            app.ModovsIRNLabel.FontSize = 20;
            app.ModovsIRNLabel.FontWeight = 'bold';
            app.ModovsIRNLabel.Position = [547 217 289 24];
            app.ModovsIRNLabel.Text = 'Modo α vs IRN';

            % Create modo_a_vs_IRN
            app.modo_a_vs_IRN = uiswitch(app.vsTab_2, 'toggle');
            app.modo_a_vs_IRN.ValueChangedFcn = createCallbackFcn(app, @modo_a_vs_IRNValueChanged, true);
            app.modo_a_vs_IRN.Position = [781 117 20 45];

            % Create ModovsINLabel
            app.ModovsINLabel = uilabel(app.vsTab_2);
            app.ModovsINLabel.HorizontalAlignment = 'center';
            app.ModovsINLabel.FontSize = 20;
            app.ModovsINLabel.FontWeight = 'bold';
            app.ModovsINLabel.Position = [547 415 290 24];
            app.ModovsINLabel.Text = 'Modo α vs IN';

            % Create modo_a_vs_IN
            app.modo_a_vs_IN = uiswitch(app.vsTab_2, 'toggle');
            app.modo_a_vs_IN.ValueChangedFcn = createCallbackFcn(app, @modo_a_vs_INValueChanged, true);
            app.modo_a_vs_IN.Position = [783 316 20 45];

            % Create ModovsLabel
            app.ModovsLabel = uilabel(app.vsTab_2);
            app.ModovsLabel.HorizontalAlignment = 'center';
            app.ModovsLabel.FontSize = 20;
            app.ModovsLabel.FontWeight = 'bold';
            app.ModovsLabel.Position = [545 608 291 24];
            app.ModovsLabel.Text = 'Modo α vs γ';

            % Create modo_alfa_vs_theta
            app.modo_alfa_vs_theta = uiswitch(app.vsTab_2, 'toggle');
            app.modo_alfa_vs_theta.ValueChangedFcn = createCallbackFcn(app, @modo_alfa_vs_thetaValueChanged, true);
            app.modo_alfa_vs_theta.Position = [785 509 20 45];

            % Create tetha_a_vs_g
            app.tetha_a_vs_g = uitextarea(app.vsTab_2);
            app.tetha_a_vs_g.FontSize = 20;
            app.tetha_a_vs_g.Position = [631 514 105 30];

            % Create Label_9
            app.Label_9 = uilabel(app.vsTab_2);
            app.Label_9.HorizontalAlignment = 'center';
            app.Label_9.FontSize = 32;
            app.Label_9.Position = [587 507 38 44];
            app.Label_9.Text = 'θ';

            % Create gama_a_vs_g
            app.gama_a_vs_g = uitextarea(app.vsTab_2);
            app.gama_a_vs_g.Editable = 'off';
            app.gama_a_vs_g.FontSize = 20;
            app.gama_a_vs_g.Position = [631 468 105 30];

            % Create alfa_a_vs_g
            app.alfa_a_vs_g = uitextarea(app.vsTab_2);
            app.alfa_a_vs_g.FontSize = 20;
            app.alfa_a_vs_g.Position = [631 560 105 30];

            % Create Label_11
            app.Label_11 = uilabel(app.vsTab_2);
            app.Label_11.HorizontalAlignment = 'center';
            app.Label_11.FontSize = 32;
            app.Label_11.Position = [594 558 25 39];
            app.Label_11.Text = 'α';

            % Create alfa_a_vs_IN
            app.alfa_a_vs_IN = uitextarea(app.vsTab_2);
            app.alfa_a_vs_IN.FontSize = 20;
            app.alfa_a_vs_IN.Position = [630 367 105 30];

            % Create TextArea_13Label
            app.TextArea_13Label = uilabel(app.vsTab_2);
            app.TextArea_13Label.HorizontalAlignment = 'center';
            app.TextArea_13Label.FontSize = 35;
            app.TextArea_13Label.Position = [592 365 38 42];
            app.TextArea_13Label.Text = 'α ';

            % Create tetha_a_vs_IN
            app.tetha_a_vs_IN = uitextarea(app.vsTab_2);
            app.tetha_a_vs_IN.FontSize = 20;
            app.tetha_a_vs_IN.Position = [630 321 105 30];

            % Create TextArea_14Label
            app.TextArea_14Label = uilabel(app.vsTab_2);
            app.TextArea_14Label.HorizontalAlignment = 'center';
            app.TextArea_14Label.FontSize = 32;
            app.TextArea_14Label.Position = [586 314 38 44];
            app.TextArea_14Label.Text = 'θ';

            % Create IN_a_vs_IN
            app.IN_a_vs_IN = uitextarea(app.vsTab_2);
            app.IN_a_vs_IN.Editable = 'off';
            app.IN_a_vs_IN.FontSize = 20;
            app.IN_a_vs_IN.Position = [630 275 105 30];

            % Create INTextAreaLabel
            app.INTextAreaLabel = uilabel(app.vsTab_2);
            app.INTextAreaLabel.HorizontalAlignment = 'center';
            app.INTextAreaLabel.FontSize = 26;
            app.INTextAreaLabel.Position = [587 269 38 42];
            app.INTextAreaLabel.Text = 'IN';

            % Create alfa_a_vs_IRN
            app.alfa_a_vs_IRN = uitextarea(app.vsTab_2);
            app.alfa_a_vs_IRN.FontSize = 20;
            app.alfa_a_vs_IRN.Position = [630 169 105 30];

            % Create TextArea_15Label
            app.TextArea_15Label = uilabel(app.vsTab_2);
            app.TextArea_15Label.HorizontalAlignment = 'center';
            app.TextArea_15Label.FontSize = 35;
            app.TextArea_15Label.Position = [592 167 38 42];
            app.TextArea_15Label.Text = 'α ';

            % Create tetha_a_vs_IRN
            app.tetha_a_vs_IRN = uitextarea(app.vsTab_2);
            app.tetha_a_vs_IRN.FontSize = 20;
            app.tetha_a_vs_IRN.Position = [630 123 105 30];

            % Create TextArea_16Label
            app.TextArea_16Label = uilabel(app.vsTab_2);
            app.TextArea_16Label.HorizontalAlignment = 'center';
            app.TextArea_16Label.FontSize = 32;
            app.TextArea_16Label.Position = [586 116 38 44];
            app.TextArea_16Label.Text = 'θ';

            % Create IRN_a_vs_IRN
            app.IRN_a_vs_IRN = uitextarea(app.vsTab_2);
            app.IRN_a_vs_IRN.Editable = 'off';
            app.IRN_a_vs_IRN.FontSize = 20;
            app.IRN_a_vs_IRN.Position = [630 77 105 30];

            % Create IRNTextAreaLabel
            app.IRNTextAreaLabel = uilabel(app.vsTab_2);
            app.IRNTextAreaLabel.HorizontalAlignment = 'center';
            app.IRNTextAreaLabel.FontSize = 26;
            app.IRNTextAreaLabel.Position = [576 71 50 42];
            app.IRNTextAreaLabel.Text = 'IRN';

            % Create CreadoporJosManuelSnchezMuozLabel_2
            app.CreadoporJosManuelSnchezMuozLabel_2 = uilabel(app.vsTab_2);
            app.CreadoporJosManuelSnchezMuozLabel_2.HorizontalAlignment = 'right';
            app.CreadoporJosManuelSnchezMuozLabel_2.FontSize = 9;
            app.CreadoporJosManuelSnchezMuozLabel_2.Position = [547 11 291 22];
            app.CreadoporJosManuelSnchezMuozLabel_2.Text = 'Creado por: José Manuel Sánchez Muñoz   ';

            % Create Label_17
            app.Label_17 = uilabel(app.vsTab_2);
            app.Label_17.FontSize = 31;
            app.Label_17.Position = [600 469 25 41];
            app.Label_17.Text = {'𝛾'; ''};

            % Create Custom_IN_IRNTab_2
            app.Custom_IN_IRNTab_2 = uitab(app.TabGroup2);
            app.Custom_IN_IRNTab_2.Title = 'Custom_IN_IRN';

            % Create alfa_vs_gama_y_corriente
            app.alfa_vs_gama_y_corriente = uiaxes(app.Custom_IN_IRNTab_2);
            title(app.alfa_vs_gama_y_corriente, 'Title')
            xlabel(app.alfa_vs_gama_y_corriente, 'X')
            ylabel(app.alfa_vs_gama_y_corriente, 'Y')
            zlabel(app.alfa_vs_gama_y_corriente, 'Z')
            app.alfa_vs_gama_y_corriente.Position = [26 435 518 202];

            % Create alfa_vs_IN_y_VL
            app.alfa_vs_IN_y_VL = uiaxes(app.Custom_IN_IRNTab_2);
            title(app.alfa_vs_IN_y_VL, 'Title')
            xlabel(app.alfa_vs_IN_y_VL, 'X')
            ylabel(app.alfa_vs_IN_y_VL, 'Y')
            zlabel(app.alfa_vs_IN_y_VL, 'Z')
            app.alfa_vs_IN_y_VL.Position = [26 233 518 202];

            % Create alfa_vs_IRN_VAK
            app.alfa_vs_IRN_VAK = uiaxes(app.Custom_IN_IRNTab_2);
            title(app.alfa_vs_IRN_VAK, 'Title')
            xlabel(app.alfa_vs_IRN_VAK, 'X')
            ylabel(app.alfa_vs_IRN_VAK, 'Y')
            zlabel(app.alfa_vs_IRN_VAK, 'Z')
            app.alfa_vs_IRN_VAK.Position = [26 25 518 202];

            % Create Label_16
            app.Label_16 = uilabel(app.Custom_IN_IRNTab_2);
            app.Label_16.FontSize = 30;
            app.Label_16.Position = [715 371 25 42];
            app.Label_16.Text = {'𝛾'; ''};

            % Create INPUTSLabel
            app.INPUTSLabel = uilabel(app.Custom_IN_IRNTab_2);
            app.INPUTSLabel.HorizontalAlignment = 'center';
            app.INPUTSLabel.FontWeight = 'bold';
            app.INPUTSLabel.Position = [546 620 289 22];
            app.INPUTSLabel.Text = 'INPUTS';

            % Create OUTPUTSLabel
            app.OUTPUTSLabel = uilabel(app.Custom_IN_IRNTab_2);
            app.OUTPUTSLabel.HorizontalAlignment = 'center';
            app.OUTPUTSLabel.FontWeight = 'bold';
            app.OUTPUTSLabel.Position = [545 463 292 22];
            app.OUTPUTSLabel.Text = 'OUTPUTS';

            % Create DispararButton_4
            app.DispararButton_4 = uibutton(app.Custom_IN_IRNTab_2, 'push');
            app.DispararButton_4.ButtonPushedFcn = createCallbackFcn(app, @Custom_IN_IRNTabButtonDown, true);
            app.DispararButton_4.BackgroundColor = [0.8 0.8 0.8];
            app.DispararButton_4.FontSize = 25;
            app.DispararButton_4.Position = [593 62 200 47];
            app.DispararButton_4.Text = {'Disparar'; ''};

            % Create mHLabel
            app.mHLabel = uilabel(app.Custom_IN_IRNTab_2);
            app.mHLabel.HorizontalAlignment = 'right';
            app.mHLabel.FontSize = 16;
            app.mHLabel.FontWeight = 'bold';
            app.mHLabel.Position = [577 488 31 22];
            app.mHLabel.Text = 'mH';

            % Create gama_out
            app.gama_out = uitextarea(app.Custom_IN_IRNTab_2);
            app.gama_out.Editable = 'off';
            app.gama_out.HorizontalAlignment = 'center';
            app.gama_out.FontSize = 15;
            app.gama_out.Position = [743 369 72 32];

            % Create alfa_out
            app.alfa_out = uitextarea(app.Custom_IN_IRNTab_2);
            app.alfa_out.Editable = 'off';
            app.alfa_out.HorizontalAlignment = 'center';
            app.alfa_out.FontSize = 15;
            app.alfa_out.Position = [607 425 72 32];

            % Create Label_3
            app.Label_3 = uilabel(app.Custom_IN_IRNTab_2);
            app.Label_3.HorizontalAlignment = 'center';
            app.Label_3.FontSize = 32;
            app.Label_3.Position = [567 423 42 39];
            app.Label_3.Text = 'α ';

            % Create IoAVGLabel
            app.IoAVGLabel = uilabel(app.Custom_IN_IRNTab_2);
            app.IoAVGLabel.HorizontalAlignment = 'center';
            app.IoAVGLabel.FontSize = 20;
            app.IoAVGLabel.FontWeight = 'bold';
            app.IoAVGLabel.Position = [588 266 70 27];
            app.IoAVGLabel.Text = 'Io AVG';

            % Create Io_AVG_out
            app.Io_AVG_out = uitextarea(app.Custom_IN_IRNTab_2);
            app.Io_AVG_out.Editable = 'off';
            app.Io_AVG_out.FontSize = 15;
            app.Io_AVG_out.Position = [568 222 109 40];

            % Create alfa_text
            app.alfa_text = uitextarea(app.Custom_IN_IRNTab_2);
            app.alfa_text.FontSize = 20;
            app.alfa_text.Position = [611 585 60 31];

            % Create Label_12
            app.Label_12 = uilabel(app.Custom_IN_IRNTab_2);
            app.Label_12.HorizontalAlignment = 'right';
            app.Label_12.FontSize = 25;
            app.Label_12.Position = [579 587 27 31];
            app.Label_12.Text = 'α ';

            % Create beta_out
            app.beta_out = uitextarea(app.Custom_IN_IRNTab_2);
            app.beta_out.Editable = 'off';
            app.beta_out.HorizontalAlignment = 'center';
            app.beta_out.FontSize = 15;
            app.beta_out.Position = [744 425 72 32];

            % Create Label_13
            app.Label_13 = uilabel(app.Custom_IN_IRNTab_2);
            app.Label_13.HorizontalAlignment = 'center';
            app.Label_13.FontSize = 28;
            app.Label_13.Position = [702 422 42 39];
            app.Label_13.Text = 'β';

            % Create teta_out
            app.teta_out = uitextarea(app.Custom_IN_IRNTab_2);
            app.teta_out.Editable = 'off';
            app.teta_out.HorizontalAlignment = 'center';
            app.teta_out.FontSize = 15;
            app.teta_out.Position = [608 368 72 32];

            % Create Label_14
            app.Label_14 = uilabel(app.Custom_IN_IRNTab_2);
            app.Label_14.HorizontalAlignment = 'center';
            app.Label_14.FontSize = 30;
            app.Label_14.Position = [564 365 42 39];
            app.Label_14.Text = 'θ';

            % Create IN_out
            app.IN_out = uitextarea(app.Custom_IN_IRNTab_2);
            app.IN_out.HorizontalAlignment = 'center';
            app.IN_out.FontSize = 15;
            app.IN_out.Position = [608 313 72 32];

            % Create INLabel
            app.INLabel = uilabel(app.Custom_IN_IRNTab_2);
            app.INLabel.HorizontalAlignment = 'center';
            app.INLabel.FontSize = 25;
            app.INLabel.Position = [565 309 42 39];
            app.INLabel.Text = 'IN';

            % Create IRN_out
            app.IRN_out = uitextarea(app.Custom_IN_IRNTab_2);
            app.IRN_out.HorizontalAlignment = 'center';
            app.IRN_out.FontSize = 15;
            app.IRN_out.Position = [743 314 72 32];

            % Create IRNLabel
            app.IRNLabel = uilabel(app.Custom_IN_IRNTab_2);
            app.IRNLabel.HorizontalAlignment = 'center';
            app.IRNLabel.FontSize = 25;
            app.IRNLabel.Position = [693 311 48 39];
            app.IRNLabel.Text = 'IRN';

            % Create IoRMSLabel_3
            app.IoRMSLabel_3 = uilabel(app.Custom_IN_IRNTab_2);
            app.IoRMSLabel_3.HorizontalAlignment = 'center';
            app.IoRMSLabel_3.FontSize = 20;
            app.IoRMSLabel_3.FontWeight = 'bold';
            app.IoRMSLabel_3.Position = [725 267 73 27];
            app.IoRMSLabel_3.Text = 'Io RMS';

            % Create Io_RMS_out
            app.Io_RMS_out = uitextarea(app.Custom_IN_IRNTab_2);
            app.Io_RMS_out.Editable = 'off';
            app.Io_RMS_out.FontSize = 15;
            app.Io_RMS_out.Position = [708 223 109 40];

            % Create VoAVGLabel_2
            app.VoAVGLabel_2 = uilabel(app.Custom_IN_IRNTab_2);
            app.VoAVGLabel_2.HorizontalAlignment = 'center';
            app.VoAVGLabel_2.FontSize = 20;
            app.VoAVGLabel_2.FontWeight = 'bold';
            app.VoAVGLabel_2.Position = [585 179 76 27];
            app.VoAVGLabel_2.Text = 'Vo AVG';

            % Create Vo_AVG_out
            app.Vo_AVG_out = uitextarea(app.Custom_IN_IRNTab_2);
            app.Vo_AVG_out.Editable = 'off';
            app.Vo_AVG_out.FontSize = 15;
            app.Vo_AVG_out.Position = [569 135 109 40];

            % Create VoRMSLabel_3
            app.VoRMSLabel_3 = uilabel(app.Custom_IN_IRNTab_2);
            app.VoRMSLabel_3.HorizontalAlignment = 'center';
            app.VoRMSLabel_3.FontSize = 20;
            app.VoRMSLabel_3.FontWeight = 'bold';
            app.VoRMSLabel_3.Position = [719 179 80 27];
            app.VoRMSLabel_3.Text = 'Vo RMS';

            % Create Vo_RMS_out
            app.Vo_RMS_out = uitextarea(app.Custom_IN_IRNTab_2);
            app.Vo_RMS_out.Editable = 'off';
            app.Vo_RMS_out.FontSize = 15;
            app.Vo_RMS_out.Position = [707 135 109 40];

            % Create Vmax_text
            app.Vmax_text = uitextarea(app.Custom_IN_IRNTab_2);
            app.Vmax_text.FontSize = 20;
            app.Vmax_text.Position = [749 585 61 31];

            % Create VmaxLabel_2
            app.VmaxLabel_2 = uilabel(app.Custom_IN_IRNTab_2);
            app.VmaxLabel_2.HorizontalAlignment = 'right';
            app.VmaxLabel_2.FontSize = 22;
            app.VmaxLabel_2.Position = [683 588 62 27];
            app.VmaxLabel_2.Text = 'Vmax';

            % Create f_text
            app.f_text = uitextarea(app.Custom_IN_IRNTab_2);
            app.f_text.FontSize = 20;
            app.f_text.Position = [611 537 60 31];

            % Create fLabel_3
            app.fLabel_3 = uilabel(app.Custom_IN_IRNTab_2);
            app.fLabel_3.HorizontalAlignment = 'right';
            app.fLabel_3.FontSize = 28;
            app.fLabel_3.Position = [570 538 25 34];
            app.fLabel_3.Text = 'f';

            % Create R_text
            app.R_text = uitextarea(app.Custom_IN_IRNTab_2);
            app.R_text.FontSize = 20;
            app.R_text.Position = [749 538 60 31];

            % Create RLabel
            app.RLabel = uilabel(app.Custom_IN_IRNTab_2);
            app.RLabel.HorizontalAlignment = 'right';
            app.RLabel.FontSize = 22;
            app.RLabel.Position = [710 539 25 27];
            app.RLabel.Text = 'R';

            % Create L_text
            app.L_text = uitextarea(app.Custom_IN_IRNTab_2);
            app.L_text.FontSize = 20;
            app.L_text.Position = [611 491 60 31];

            % Create LLabel_2
            app.LLabel_2 = uilabel(app.Custom_IN_IRNTab_2);
            app.LLabel_2.HorizontalAlignment = 'right';
            app.LLabel_2.FontSize = 22;
            app.LLabel_2.Position = [556 488 25 27];
            app.LLabel_2.Text = 'L';

            % Create CreadoporJosManuelSnchezMuozLabel_3
            app.CreadoporJosManuelSnchezMuozLabel_3 = uilabel(app.Custom_IN_IRNTab_2);
            app.CreadoporJosManuelSnchezMuozLabel_3.HorizontalAlignment = 'right';
            app.CreadoporJosManuelSnchezMuozLabel_3.FontSize = 9;
            app.CreadoporJosManuelSnchezMuozLabel_3.Position = [548 5 291 22];
            app.CreadoporJosManuelSnchezMuozLabel_3.Text = 'Creado por: José Manuel Sánchez Muñoz   ';

            % Show the figure after all components are created
            app.UIFigure.Visible = 'on';
        end
    end

    % App creation and deletion
    methods (Access = public)

        % Construct app
        function app = GUI_Terminada

            % Create UIFigure and components
            createComponents(app)

            % Register the app with App Designer
            registerApp(app, app.UIFigure)

            % Execute the startup function
            runStartupFcn(app, @startupFcn)

            if nargout == 0
                clear app
            end
        end

        % Code that executes before app deletion
        function delete(app)

            % Delete UIFigure when app is deleted
            delete(app.UIFigure)
        end
    end
end
